# Medusa

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Medusa is an open-source, MIT-licensed digital commerce platform built around a modular architecture: a suite of Commerce Modules (cart, products, orders, pricing, promotions, tax, inventory, fulfillment, payment), a Framework for building custom API routes, data models, workflows and integrations, and a customizable Medusa Admin dashboard. Medusa ships two first-party REST APIs — a Store API for storefronts and an Admin API for merchant operations — both documented with published OpenAPI 3.0 specifications generated from the codebase. Medusa is self-hosted by default; MedusaJS, Inc. also operates Medusa Cloud, a managed PaaS, and a remote MCP server plus published Claude Code agent skills for agentic development.

**Areas:** E-Commerce · Headless Commerce · Open Source · Commerce · Storefront · Order Management · Node.js · GraphQL · Agentic Commerce · MCP

## Medusa on APIs.io

Everything profiled for Medusa is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/medusa/](https://apis.io/providers/medusa/)** — or go straight to one of the APIs or properties below.

### APIs (72)

- [Medusa GraphQL API](https://apis.io/apis/medusa/medusa-graphql-api/) — Medusa's GraphQL surface over the store data core. The schema in this repo was derived from the OAS output schemas published in the medusajs/medusa…
- [Medusa MCP Remote Server](https://apis.io/apis/medusa/medusa-mcp-server/) — Medusa hosts a Streamable HTTP Model Context Protocol server at https://docs.medusajs.com/mcp. It exposes the Medusa documentation to coding agents plus…
- [Medusa Api Keys API](https://apis.io/apis/medusa/medusa-api-keys-api/) — API keys can be used for authentication or resource-scoping. A secret API key can be used to authenticate admin users. A publishable API key can be used to…
- [Medusa Auth API](https://apis.io/apis/medusa/medusa-auth-api/) — Auth API routes allow you to manage an admin user's authentication.
- [Medusa [auth Provider] API](https://apis.io/apis/medusa/medusa-auth-provider-api/) — The [auth_provider] API from Medusa — 1 operation(s) for [auth_provider].
- [Medusa Campaigns API](https://apis.io/apis/medusa/medusa-campaigns-api/) — A campaign is a group of promotions that have the same conditions, such as start and end dates. These API routes allow admin users to manage campaigns,…
- [Medusa Carts API](https://apis.io/apis/medusa/medusa-carts-api/) — A cart is a virtual shopping bag that customers can use to add items they want to purchase. A cart is then used to checkout and place an order. These API…
- [Medusa Claims API](https://apis.io/apis/medusa/medusa-claims-api/) — An admin creates a claim for an order when a customer reports that an item is defective or incorrect. Using these API routes, admin users manage order…
- [Medusa Collections API](https://apis.io/apis/medusa/medusa-collections-api/) — A product collection organizes products into a collection for marketing purposes. For example, a summer collection. These API routes allow admin users to…
- [Medusa Currencies API](https://apis.io/apis/medusa/medusa-currencies-api/) — A store can use unlimited currencies, and each region must be associated with at least one currency. Currencies are defined by the Currency Module. Currency…
- [Medusa Customer Groups API](https://apis.io/apis/medusa/medusa-customer-groups-api/) — Customers can be organized into groups. These groups are useful for segregation and marketing purposes. For example, you can provide different prices for…
- [Medusa Customers API](https://apis.io/apis/medusa/medusa-customers-api/) — Customers can either be created when they register through the Store APIs, or created by the admin using the Admin APIs. These API routes allow admin users…
- [Medusa Draft Orders API](https://apis.io/apis/medusa/medusa-draft-orders-api/) — A draft order is an order created by the admin user. This is useful for orders created offline or from clients other than a storefront, such as a…
- [Medusa Exchanges API](https://apis.io/apis/medusa/medusa-exchanges-api/) — An exchange is the replacement of an item that the customer ordered with another. These API routes allow admin users to create and manage exchanges.
- [Medusa Feature Flags API](https://apis.io/apis/medusa/medusa-feature-flags-api/) — Feature flags are used to enable or disable certain features in your Medusa application. These API routes allow admin users to view feature flags.
- [Medusa Fulfillment Providers API](https://apis.io/apis/medusa/medusa-fulfillment-providers-api/) — A fulfillment provider is a third-party integration or custom logic used to fulfill an order's items. Fulfillment providers are installed as module providers.
- [Medusa Fulfillment Sets API](https://apis.io/apis/medusa/medusa-fulfillment-sets-api/) — A fulfillment set is a general form or way of fulfillment, such as "shipping" or "pick up". All fulfillment-related configurations in a store are related to…
- [Medusa Fulfillments API](https://apis.io/apis/medusa/medusa-fulfillments-api/) — A fulfillment is created for items in an order, return, exchanges, or claims to deliver items to/from the customer. These API routes allow admin users to…
- [Medusa Gift Cards API](https://apis.io/apis/medusa/medusa-gift-cards-api/) — A gift card is a prepaid card that can be used to pay for items during checkout. Gift cards can be purchased by customers, or created by admin users. When a…
- [Medusa Index API](https://apis.io/apis/medusa/medusa-index-api/) — The Index Module is a tool to perform high-performance queries across modules, for example, to filter linked modules. The Index Module is currently…
- [Medusa Inventory Items API](https://apis.io/apis/medusa/medusa-inventory-items-api/) — An inventory item is a stock-kept product whose inventory is managed. These API routes allow admin users to manage inventory items.
- [Medusa Invites API](https://apis.io/apis/medusa/medusa-invites-api/) — An admin can invite new users to manage their team. This allows new users to authenticate as admins and perform admin functionalities. These API routes…
- [Medusa Layouts API](https://apis.io/apis/medusa/medusa-layouts-api/) — An admin can modify the layout of their admin dashboard. This allows admins to customize their dashboard to their preferences and needs. These API routes…
- [Medusa Locales API](https://apis.io/apis/medusa/medusa-locales-api/) — A locale is a language that content is translated into for customers to view in a storefront. Medusa installs locales by default. These API routes allow…
- [Medusa Multi-Factor Authentication API](https://apis.io/apis/medusa/medusa-multi-factor-authentication-api/) — Multi-factor authentication (MFA) adds an extra layer of security to admin accounts by requiring additional verification factors during login, such as a…
- [Medusa Multi-Factor Authentication (MFA) Factors API](https://apis.io/apis/medusa/medusa-multi-factor-authentication-mfa-factors-api/) — Multi-factor authentication (MFA) factors are additional ways to verify a customer's identity during login, in addition to their password. Examples of MFA…
- [Medusa Notifications API](https://apis.io/apis/medusa/medusa-notifications-api/) — A notification informs an admin user of store changes or status changes of background tasks. These API routes allow admin users to view and manage…
- [Medusa Order Changes API](https://apis.io/apis/medusa/medusa-order-changes-api/) — An order change is a proposed change to an order, such as adding or removing items, changing shipping methods, and more. They can be associated with order…
- [Medusa Order Edits API](https://apis.io/apis/medusa/medusa-order-edits-api/) — An order edit is a change to an order's details, such as items, shipping methods, and more. Changes made by an order edit are only applied on the order once…
- [Medusa Orders API](https://apis.io/apis/medusa/medusa-orders-api/) — An order is a purchase made by a customer through a storefront. Orders can also originally be created as draft orders. These API routes allow admin users to…
- [Medusa Payment Collections API](https://apis.io/apis/medusa/medusa-payment-collections-api/) — A payment collection is one or more payments of an order. They're also used for outstanding payments due to order exchanges or claims. Every purchase or…
- [Medusa Payment Providers API](https://apis.io/apis/medusa/medusa-payment-providers-api/) — Each region has a set of payment providers enabled. During checkout, you retrieve the available payment providers in the customer's region to show them to…
- [Medusa Payments API](https://apis.io/apis/medusa/medusa-payments-api/) — A payment is created when a payment amount is authorized. The payment can then be captured or refunded. A payment is created from the payment session that…
- [Medusa Plugins API](https://apis.io/apis/medusa/medusa-plugins-api/) — A plugin is a package of reusable Medusa customizations that you can install in any Medusa application. Plugins can be used to add new functionality, such…
- [Medusa Price Lists API](https://apis.io/apis/medusa/medusa-price-lists-api/) — A price list is a group of prices applied if the specified conditions and rules are satisfied. Price lists are useful for sales or special prices for…
- [Medusa Price Preferences API](https://apis.io/apis/medusa/medusa-price-preferences-api/) — A price preference is used to specify whether tax-inclusiveness is enabled for a context, such as a region or currency code. These API routes allow admin…
- [Medusa Product Categories API](https://apis.io/apis/medusa/medusa-product-categories-api/) — Products can be categorized into categories. Categories are nested and their heirarchy can be managed, giving admin users flexibility in how they categorize…
- [Medusa Product Options API](https://apis.io/apis/medusa/medusa-product-options-api/) — A product option is a way to define different options for a product, such as "Size" or "Color". Product options can be created globally and used by multiple…
- [Medusa Product Tags API](https://apis.io/apis/medusa/medusa-product-tags-api/) — A tag is another way of organizing a product. Each tag has a name and a value. Products are organized into the same tag if they have the same value. These…
- [Medusa Product Types API](https://apis.io/apis/medusa/medusa-product-types-api/) — Products can be organized into types. Each type has a name and a value. Products are organized into the same type if they have the same value. These API…
- [Medusa Product Variants API](https://apis.io/apis/medusa/medusa-product-variants-api/) — A product variant is a saleable form of the product. Each variant has different option values. For example, a "Shirt" product may have a "Blue" variant and…
- [Medusa Products API](https://apis.io/apis/medusa/medusa-products-api/) — A product is a set of variants that the customer chooses from when making a purchase. A product can be organized into categories or collections. A product…
- [Medusa Promotions API](https://apis.io/apis/medusa/medusa-promotions-api/) — A promotion discounts an amount or percentage off a cart's items, shipping methods, or the entire order. Promotions have different types, such as a…
- [Medusa Property Labels API](https://apis.io/apis/medusa/medusa-property-labels-api/) — The Property Labels API from Medusa — 3 operation(s) for property labels.
- [Medusa Refund Reasons API](https://apis.io/apis/medusa/medusa-refund-reasons-api/) — A refund reason is a possible reason used when issuing a refund to the customer, such as when returning an item and refunding the customer. These API routes…
- [Medusa Regions API](https://apis.io/apis/medusa/medusa-regions-api/) — Regions are different countries or geographical regions that the commerce store serves customers in. These API routes allow admin users to manage regions,…
- [Medusa Reservations API](https://apis.io/apis/medusa/medusa-reservations-api/) — A reservation is unavailable quantity of an inventory item in a location. A reservation is created automatically for variants in an order whose…
- [Medusa Return Reasons API](https://apis.io/apis/medusa/medusa-return-reasons-api/) — A return reason is a possible reason that an item is returned from the customer, such as when returning an item. These API routes allow admin users to…
- [Medusa Returns API](https://apis.io/apis/medusa/medusa-returns-api/) — Admin users create a return when a customer returns an item to them. Returns can also be created by customers through the storefront, and admins will be…
- [Medusa Sales Channels API](https://apis.io/apis/medusa/medusa-sales-channels-api/) — A sales channel indicates a channel where products can be sold in. For example, a webshop or a mobile app. These API routes allow admins to manage sales…
- [Medusa Search API](https://apis.io/apis/medusa/medusa-search-api/) — The Search API from Medusa — 1 operation(s) for search.
- [Medusa Shipping Option Types API](https://apis.io/apis/medusa/medusa-shipping-option-types-api/) — Shipping option types define a group of shipping options with shared shipping characterstics. For example, you may have "Standard" and "Express" shipping…
- [Medusa Shipping Options API](https://apis.io/apis/medusa/medusa-shipping-options-api/) — A shipping option is a way of shipping an item to or from the customer. Shipping options are associated with the fulfillment provider used to handle their…
- [Medusa Shipping Profiles API](https://apis.io/apis/medusa/medusa-shipping-profiles-api/) — A shipping profile defines a type of items that are shipping in a similar manner. For example, digital products may have a `digital` shipping profile. These…
- [Medusa Stock Locations API](https://apis.io/apis/medusa/medusa-stock-locations-api/) — A stock location is where stock-kept items (products) are kept. Stock locations are linked to fulfillment providers used to fulfill items from this…
- [Medusa Store Credit Accounts API](https://apis.io/apis/medusa/medusa-store-credit-accounts-api/) — A store credit account is a ledger of store credit transactions for a customer. They hold the customer's store credit balance, including their credit and…
- [Medusa Stores API](https://apis.io/apis/medusa/medusa-stores-api/) — A store holds the main configuration and information of your commerce store, such as supported currencies or default sales channel. By default, the Medusa…
- [Medusa Tax Providers API](https://apis.io/apis/medusa/medusa-tax-providers-api/) — A tax provider is a third-party integration or custom logic used to calculate taxes for a cart or an order. These API routes allow admin users to manage tax…
- [Medusa Tax Rates API](https://apis.io/apis/medusa/medusa-tax-rates-api/) — A tax rate is a percentage amount used to calculate the tax amount of each taxable item's price, such as line items or shipping methods. Each tax region has…
- [Medusa Tax Regions API](https://apis.io/apis/medusa/medusa-tax-regions-api/) — A tax region is a region's tax settings. It has tax rates and rules. So, after you create a region, you must create a tax region for it. A tax region can…
- [Medusa Translations API](https://apis.io/apis/medusa/medusa-translations-api/) — A translation is a localized version of content in a specific locale. For example, a product description in French. These API routes allow admin users to…
- [Medusa Uploads API](https://apis.io/apis/medusa/medusa-uploads-api/) — Use these API routes to upload files to your Medusa application using the installed file module provider. You can upload public files, such as product…
- [Medusa Users API](https://apis.io/apis/medusa/medusa-users-api/) — A user is an admin user that can authenticate and perform functionalities as an admin user. An admin user can invite other users to join their team. Once…
- [Medusa Views API](https://apis.io/apis/medusa/medusa-views-api/) — A view configuration is a saved data-table view for an entity, such as products or orders. It lets admin users customize how a table shows its data, then…
- [Medusa Workflows Executions API](https://apis.io/apis/medusa/medusa-workflows-executions-api/) — These API routes allow you to track workflow executions in your Medusa application. Depending on the workflow engine you use, executions may only be…
- [Medusa JS SDK (@medusajs/js-sdk)](https://apis.io/apis/medusa/js-sdk/) — Official TypeScript / JavaScript SDK wrapping the Store and Admin REST APIs - typed clients, auth helpers, and ergonomic resource methods. Distributed via…
- [Medusa Framework (Modules, Workflows, Routes)](https://apis.io/apis/medusa/framework/) — Server-side framework primitives for extending Medusa - custom API Routes, Modules with their own data models (DML), Module Links, Workflows for…
- [Medusa Commerce Modules](https://apis.io/apis/medusa/commerce-modules/) — First-party domain modules that compose into a Medusa application - Cart, Payment, Customer, Pricing, Promotion, Product, Order, Inventory, Fulfillment,…
- [Medusa CLI (create-medusa-app)](https://apis.io/apis/medusa/cli/) — Command-line tooling for scaffolding new Medusa projects, generating modules and migrations, running the server in dev, and managing common project tasks.
- [Medusa Next.js Storefront Starter](https://apis.io/apis/medusa/nextjs-starter/) — Reference Next.js storefront talking to the Medusa Store API - cart, checkout, account, product browse, payments, and search. Used as the canonical starting…
- [Medusa Docs MCP Server](https://apis.io/apis/medusa/mcp-server/) — Remote Model Context Protocol server exposing the Medusa documentation to LLM-powered coding assistants - lets agents look up commerce modules, framework…
- [Medusa Core Repository](https://apis.io/apis/medusa/core-repo/) — Monorepo with the Medusa server, Admin, Commerce Modules, Framework, and packages. MIT-licensed reference for self-hosting and for building modules and plugins.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Medusa Events](https://apis.io/asyncapis/medusa/medusa-events/)

#### GraphQL (1)

GraphQL schemas.

- [Medusa GraphQL API](https://apis.io/graphqls/medusa/medusa-graphql/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [medusa](https://apis.io/servers/medusa/medusa/)

#### Overlays (2)

OpenAPI overlays, including conversational phrasing for each operation.

- [Medusa Admin Overlay](https://apis.io/overlays/medusa/medusa-admin-overlay/)
- [Medusa Store Overlay](https://apis.io/overlays/medusa/medusa-store-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Medusa Authentication](https://apis.io/security/medusa/medusa-authentication/)
- [Medusa Domain Security](https://apis.io/security/medusa/medusa-domain-security/)
- [Medusa Vulnerability Disclosure](https://apis.io/security/medusa/medusa-vulnerability-disclosure/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Medusa Scopes](https://apis.io/scopes/medusa/medusa-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Medusa Plans Pricing](https://apis.io/plans/medusa/medusa-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Medusa Rate Limits](https://apis.io/rate-limits/medusa/medusa-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://medusajs.com/)
- [Documentation](https://docs.medusajs.com/learn)
- [Getting started](https://docs.medusajs.com/learn/installation)
- [API reference](https://docs.medusajs.com/api/store)
- [Pricing](https://medusajs.com/pricing)
- [Sign up](https://cloud.medusajs.com/signup)
- [Support](https://medusajs.com/contact/)
- [Blog](https://medusajs.com/blog/)
- [Security](https://github.com/medusajs/medusa/security/policy)
- [Terms of service](https://medusajs.com/terms-of-service)
- [Privacy policy](https://medusajs.com/privacy-policy)
- [GitHub](https://github.com/medusajs)
- [Status](https://status.medusajs.com)

## API Evangelist rating

**Kin Score 66.0** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 75.0 |
| Contract quality | 57.9 |
| Contract governance | 4.5 |
| Operational transparency | 60.5 |
| Developer ergonomics | 85.7 |
| Access clarity | 63.2 |

**Agent readiness 59.1** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | documented (partial credit) |
| MCP Server | verified |
| Auth Clarity | served (partial credit) |
| Idempotency | documented (partial credit) |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | partial |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | yes |
| Agent Skills | yes |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | verified |
| Dynamic Client Registration | yes |
| Agentic Commerce | — |
| Pagination Ratio | paginated |
| Operation Distinctiveness | — |

**Regulatory alignment 40.2** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/medusa/](https://apis.io/providers/medusa/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Medusa: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/medusa/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
