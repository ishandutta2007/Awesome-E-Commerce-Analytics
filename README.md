# Awesome-E-Commerce-Analytics

# Top E-commerce Analytics Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Profit Attribution, Customer Cohorts & Self-Hosted Commerce Intelligence*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **E-commerce Analytics**. These tools enable merchants to go beyond basic traffic and sales reports—connecting marketing spend, product costs, and customer behavior to reveal true profitability, lifetime value, and the levers that actually drive growth.

**Examples** include Shopify Reports and Analytics, Triple Whale, Lifetimely, Polar Analytics, Daasity, Glew.io, Looker, Google Analytics 4, Mixpanel, and Metabase (the category leaders).

**Open-source emphasis**: E-commerce Analytics is a domain where open-source tooling is **emerging but still catching up to the integrated, store-aware SaaS platforms**. The strongest active project is **OverSeek**, a self-hosted operations hub for WooCommerce that unifies analytics, inventory, marketing, and customer intelligence in one dashboard with Docker deployment . For general-purpose analytics, **Metabase** provides a solid foundation for building custom e-commerce dashboards from synced store data, with pre-built templates for net revenue, orders, AOV, and channel mix . However, **no open-source project matches the plug-and-play profitability attribution and cohort analysis** of Triple Whale or Lifetimely out of the box—those platforms derive signal from integrated pixel tracking, ad platform connections, and pre-built LTV models that require significant custom development to replicate.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Shopify Reports and Analytics](https://www.shopify.com/)**  
  Native analytics within Shopify Admin with reports covering acquisition (sessions by referrer, location), behavior (conversion rate, cart analysis, popular searches), customers (first-time vs returning, at-risk, loyal), inventory, and finance; custom reports available on Basic and higher plans . **Free and foundational**, but limited to Shopify data and lacks cross-channel ad spend attribution.

- **[Triple Whale](https://www.triplewhale.com/)**  
  All-in-one e-commerce analytics and business intelligence platform for Shopify, WooCommerce, and BigCommerce brands . Features **first-party pixel and attribution**, Sonar enrichment, AI assistant (Moby) for forecasting and visualizations, 50+ dashboard templates, **Multi-Shop Dashboard** for portfolio comparison, external revenue import (retail/wholesale/offline), and **Data Warehouse Export** to BigQuery, Snowflake, or S3 . Positioned as a single source of truth for scaling DTC brands.

- **[Lifetimely](https://www.lifetimely.io/)**  
  Shopify app specializing in **profit and LTV analytics**; provides automated P&L reports integrated with 10+ marketing and shipping platforms, accurate LTV projections, advanced cohort analysis, CAC payback calculators, and monthly revenue projections . Users praise the depth of customer and product insights, noting it answers questions Shopify or Google Analytics alone cannot .

- **[Polar Analytics](https://www.polaranalytics.com/)**  
  AI-native analytics platform that positions itself as a **data foundation for agents**; connects commerce, marketing, inventory, and finance data into Snowflake, with a semantic layer ensuring metric definitions are consistent across answers . Features Ask Polar (natural language queries with root-cause analysis), AI agents for monitoring plans and ad spend, and MCP integration for compatible AI assistants. Users highlight plug-and-play setup, multi-shop dashboards, and responsive support .

- **[Daasity](https://www.daasity.com/)**  
  Unified commerce data platform with ELT into a data warehouse, pre-built data models, and a drag-and-drop Explore interface for custom reports . Features dashboards for Total Company, E-commerce, Retail, and Marketing; **Audiences** for pushing customer segments back to Meta, Google, Klaviyo, and Braze (Reverse ETL); 50+ integrations; and a Templates Library with cohort analysis, marketing attribution, inventory analytics, and promotional analysis.

- **[Glew.io](https://www.glew.io/)**  
  Multichannel commerce intelligence platform connecting Shopify with Google Analytics, Amazon, Facebook, Google Ads, Recharge, and 100+ other sources . Provides unified reporting on marketing channels, customers, products, and inventory; pre-built and custom segments; subscription analytics via Recharge integration; and unlimited users and historical data.

- **[Looker](https://looker.com/)**  
  Google Cloud BI platform built on LookML for governed, reusable metric definitions; strongest when standardized on BigQuery and paired with a data warehouse for custom e-commerce analytics.

- **[Google Analytics 4](https://analytics.google.com/)**  
  Web and app analytics with e-commerce event tracking, funnel exploration, and audience building; free but increasingly complex and limited for deep profitability analysis without additional tooling.

- **[Mixpanel](https://mixpanel.com/)**  
  Product analytics platform with event tracking, funnels, retention, and cohort analysis; useful for behavioral analysis but requires custom instrumentation for e-commerce specific metrics.

- **[Metabase](https://www.metabase.com/)**  
  Open-source BI tool (listed here for its managed cloud option) with an e-commerce sales dashboard template covering net revenue, orders, AOV, refund rate, and channel/region mix . Requires syncing store data into a database and defining metrics.

## Open-Source GitHub Projects

### Self-Hosted E-commerce Operations Hubs

- **[OverSeek](https://github.com/MerlinStacks/overseek)**  
  The most comprehensive open-source **self-hosted operations hub for WooCommerce** . Syncs store data into PostgreSQL with real-time tracking; features a custom dashboard with drag-and-drop widgets for revenue, live visitors, inbox, SEO, and ads; **orders and abandoned carts** with COGS and attribution; **analytics** including revenue, attribution, cohorts, CLV, and conversion API health; **growth** modules for paid ads, reviews, SEO, and product feeds; email marketing; inventory and supply chain; and a mobile PWA. Docker Compose deployment. **The strongest open-source starting point for WooCommerce merchants** wanting unified commerce intelligence, though it is WooCommerce-specific and newer than established SaaS platforms.

### General-Purpose BI (Build Your Own E-commerce Dashboard)

- **[Metabase](https://github.com/metabase/metabase)**  
  Leading open-source BI platform (AGPL) with an **e-commerce sales dashboard template** covering net revenue, orders, AOV, refund rate, revenue by week (with prior-period comparison), revenue by channel/region/discount status, and top products . Sync Shopify, WooCommerce, or BigCommerce data into a database, define net revenue once, and build governed dashboards. **The most accessible open-source foundation for custom e-commerce analytics**—requires SQL fluency and data modeling but provides full control over metrics and definitions.

- **[Apache Superset](https://github.com/apache/superset)**  
  Open-source BI platform (Apache 2.0) with 40+ chart types, SQL Lab, and enterprise RBAC; heavier infrastructure than Metabase but more scalable for large data volumes. **For teams with dedicated analytics engineering capacity** building custom commerce dashboards.

### Additional Strong Open-Source Options

- **rabbit-analytics** — A custom analytics service for Shopify and WooCommerce platforms (npm package, MIT); small scope but useful as a starting point for custom event tracking .
- **No mature open-source equivalent to Triple Whale or Lifetimely exists** — The first-party pixel tracking, ad platform attribution, LTV modeling, and AI-powered forecasting of these platforms are not replicated by any active open-source project. OverSeek covers WooCommerce operations but not the multi-channel ad attribution and cohort profitability depth of the commercial leaders.

**Frameworks for building custom systems**: For **WooCommerce merchants**, OverSeek provides a unified operations hub with analytics, inventory, and marketing . For **custom dashboards across any platform**, combine Metabase or Superset with a data warehouse (PostgreSQL, BigQuery, Snowflake) and define your own metrics . For **profitability and LTV depth**, no open-source project matches Lifetimely or Triple Whale—organizations requiring these insights should evaluate commercial platforms or invest in custom data modeling.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- E-commerce analytics platforms handling customer and transaction data must comply with applicable privacy regulations (GDPR, CCPA) and implement proper consent mechanisms for tracking pixels and cookies.
- **Open-source e-commerce analytics is strongest as a foundation, not a turnkey solution**—OverSeek provides a unified WooCommerce hub , and Metabase provides BI primitives for custom dashboards . However, **no open-source project replicates the integrated profit attribution, LTV modeling, and AI forecasting** of Triple Whale or Lifetimely. Merchants requiring these insights should evaluate commercial platforms or invest in custom data pipelines.
- Verify license terms for commercial use; OverSeek is open-source (check repository), Metabase uses AGPL with paid Pro/Enterprise tiers, and Superset uses Apache 2.0.

---

**Made for e-commerce operators, growth teams, finance analysts, and data-driven merchants.**  
Let's make e-commerce analytics more open, but with clear eyes about the profitability and attribution depth that commercial platforms still lead on.
