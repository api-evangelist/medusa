# Medusa GraphQL API

Medusa is an open-source headless commerce platform with a modular architecture that enables developers to build custom commerce applications. The GraphQL API exposes the full store surface for building storefronts.

- **Docs**: https://docs.medusajs.com
- **Store API Reference**: https://docs.medusajs.com/api/store
- **Base URL**: `https://{medusa-backend-domain}/store/graphql`
- **GitHub**: https://github.com/medusajs/medusa
- **License**: MIT

## Schema Source

Schema derived from the official OAS (OpenAPI Specification) output schemas published in the `medusajs/medusa` repository (`develop` branch) under `www/utils/generated/oas-output/schemas/`. Medusa's core GraphQL utilities live in `packages/core/utils/src/graphql/` and use a code-generation pipeline (`gqlSchemaToTypes`) that converts GraphQL SDL into TypeScript types.

## Authentication

The store API supports two authentication modes:

- **JWT Bearer token** — Include `Authorization: Bearer <token>` header after logging in.
- **Cookie session** — Session-based auth for browser clients.

Customer registration and login are handled via `/store/auth` REST routes. Authenticated mutations (cart completion, customer profile, orders, returns) require a valid session or token.

## Core Types

| Type | Description |
|---|---|
| `Product` | A store product with variants, options, images, tags, and categories |
| `ProductVariant` | A specific purchasable variant of a product (SKU, price, dimensions) |
| `ProductOption` | A product option axis such as Size or Color |
| `ProductOptionValue` | A concrete value for a product option (e.g. "Large", "Red") |
| `ProductImage` | Product image with URL and rank |
| `ProductTag` | Keyword tag attached to a product |
| `ProductType` | Product classification type |
| `ProductCategory` | Hierarchical product category (supports parent/child nesting) |
| `ProductCollection` | A curated collection of products |
| `Cart` | Shopping cart with line items, shipping methods, promotions, and totals |
| `CartLineItem` | A product variant and quantity in a cart, with computed totals |
| `CartShippingMethod` | A shipping method applied to a cart |
| `CartPromotion` | A promotion code applied to a cart |
| `PaymentCollection` | Groups payment sessions for a cart |
| `PaymentSession` | A payment attempt via a specific provider |
| `PaymentProvider` | An enabled payment provider (e.g. Stripe) |
| `Order` | A placed order with line items, shipping, fulfillments, and financial totals |
| `OrderLineItem` | A line item in an order with tax lines and adjustments |
| `OrderShippingMethod` | Shipping method applied to an order |
| `OrderFulfillment` | Fulfillment record for shipped items |
| `OrderSummary` | Aggregated financial summary for an order |
| `Customer` | A registered store customer |
| `CustomerAddress` | A saved address on a customer profile |
| `Address` | A cart or order address |
| `Region` | A geographic commerce region with currency and payment providers |
| `Country` | A country within a region |
| `Currency` | A supported currency |
| `StoreCurrency` | Currency configuration per store (tax-inclusive flag) |
| `ShippingOption` | An available shipping method a customer can select |
| `ShippingOptionType` | Classification of a shipping option |
| `Return` | A return request on an order |
| `ReturnItem` | A line item being returned |
| `ReturnReason` | A reason category for a return |
| `GiftCard` | A gift card with balance and status |
| `Price` | A price set entry with currency, amount, and quantity rules |
| `PriceRule` | A conditional rule that governs price applicability |
| `CalculatedPrice` | The resolved price for a variant or shipping option in context |
| `MoneyAmount` | A currency/amount pair |
| `Store` | Store configuration with supported currencies and defaults |

## Enums

| Enum | Values |
|---|---|
| `ProductStatus` | `draft`, `proposed`, `published`, `rejected` |
| `GiftCardStatus` | `disabled`, `enabled` |
| `ReturnStatus` | `open`, `requested`, `received`, `partially_received`, `canceled` |
| `OrderStatus` | `pending`, `completed`, `archived`, `canceled`, `requires_action` |
| `PaymentStatus` | `not_paid`, `awaiting`, `captured`, `partially_captured`, `partially_refunded`, `refunded`, `canceled`, `requires_action` |
| `FulfillmentStatus` | `not_fulfilled`, `partially_fulfilled`, `fulfilled`, `partially_shipped`, `shipped`, `partially_delivered`, `delivered`, `canceled` |
| `PaymentSessionStatus` | `authorized`, `captured`, `pending`, `requires_more`, `error`, `canceled` |
| `ShippingOptionPriceType` | `flat`, `calculated` |
| `PriceRuleOperator` | `eq`, `ne`, `gt`, `gte`, `lt`, `lte`, `in`, `nin` |

## Queries

| Query | Description |
|---|---|
| `products(...)` | List products with filtering by ID, handle, collection, category, tag, type, sales channel, region, and status |
| `product(id, handle)` | Retrieve a single product |
| `productVariants(...)` | List product variants |
| `productVariant(id)` | Retrieve a single variant |
| `collections(...)` | List product collections |
| `collection(id, handle)` | Retrieve a single collection |
| `productCategories(...)` | List product categories with ancestor/descendant tree options |
| `productCategory(id, handle)` | Retrieve a single category |
| `productTags(...)` | List product tags |
| `productTypes(...)` | List product types |
| `regions(...)` | List regions |
| `region(id)` | Retrieve a single region |
| `currencies(...)` | List currencies |
| `currency(code)` | Retrieve a single currency |
| `shippingOptions(...)` | List shipping options for a cart or return |
| `returnReasons(...)` | List return reasons |
| `returnReason(id)` | Retrieve a single return reason |
| `cart(id)` | Retrieve a cart |
| `order(id, display_id)` | Retrieve an order |
| `orders(...)` | List authenticated customer orders |
| `customer` | Retrieve the authenticated customer |
| `customerAddresses(...)` | List authenticated customer addresses |
| `paymentCollection(id)` | Retrieve a payment collection |
| `paymentProviders(region_id)` | List available payment providers for a region |
| `store` | Retrieve store configuration |
| `giftCard(code)` | Retrieve a gift card by code |
| `return(id)` | Retrieve a return |

## Mutations

| Mutation | Description |
|---|---|
| `createCart(input)` | Create a new shopping cart |
| `updateCart(id, input)` | Update cart details (region, email, addresses, promo codes) |
| `addCartLineItem(...)` | Add a product variant to the cart |
| `updateCartLineItem(...)` | Update quantity of a cart line item |
| `removeCartLineItem(...)` | Remove a line item from the cart |
| `addCartPromotions(...)` | Apply promotion codes to the cart |
| `removeCartPromotion(...)` | Remove a promotion code from the cart |
| `addGiftCardToCart(...)` | Apply a gift card to the cart |
| `removeGiftCardFromCart(...)` | Remove a gift card from the cart |
| `createPaymentCollection(...)` | Create a payment collection for checkout |
| `initializePaymentSession(...)` | Initialize a provider payment session |
| `completeCart(id)` | Complete checkout and place an order |
| `createCustomer(input)` | Register a new customer account |
| `updateCustomer(input)` | Update the authenticated customer profile |
| `createCustomerAddress(input)` | Add an address to the customer profile |
| `updateCustomerAddress(...)` | Update a customer address |
| `deleteCustomerAddress(...)` | Remove a customer address |
| `requestOrderTransfer(...)` | Request to transfer an order to another customer |
| `acceptOrderTransfer(...)` | Accept an incoming order transfer |
| `declineOrderTransfer(...)` | Decline an incoming order transfer |
| `createReturn(input)` | Submit a return request for an order |
| `claimStoreCreditAccount(token)` | Claim a store credit account via token |

## Example Queries

### Fetch Products

```graphql
query ListProducts {
  products(limit: 10, status: [published]) {
    products {
      id
      title
      handle
      thumbnail
      status
      variants {
        id
        title
        sku
        calculated_price {
          calculated_amount
          currency_code
        }
      }
      options {
        id
        title
        values {
          id
          value
        }
      }
      images {
        url
      }
    }
    count
    offset
    limit
  }
}
```

### Create and Complete a Cart

```graphql
mutation CreateCart {
  createCart(input: {
    region_id: "reg_01HV..."
    items: [
      { variant_id: "variant_01HV...", quantity: 1 }
    ]
  }) {
    id
    items {
      id
      title
      quantity
      unit_price
      total
    }
    total
    currency_code
  }
}

mutation CompleteCart {
  completeCart(id: "cart_01HV...") {
    id
    status
    total
    currency_code
    email
  }
}
```

### Register a Customer

```graphql
mutation Register {
  createCustomer(input: {
    email: "customer@example.com"
    password: "strongpassword"
    first_name: "Jane"
    last_name: "Doe"
  }) {
    id
    email
    first_name
    last_name
  }
}
```

### Create a Return

```graphql
mutation CreateReturn {
  createReturn(input: {
    order_id: "order_01HV..."
    items: [
      { id: "item_01HV...", quantity: 1, reason_id: "rr_01HV...", note: "Wrong size" }
    ]
    shipping: { option_id: "so_01HV..." }
  }) {
    id
    status
    items {
      id
      quantity
      reason {
        label
      }
    }
  }
}
```
