# UCP // Fluent — Privacy Policy

**Last updated: July 11, 2026**

This Privacy Policy explains how **Aurina AI LLC**, doing business as **UCP // Fluent** ("UCP Fluent," "we," "us"), handles data when a Shopify merchant ("you," "Merchant") installs and uses the UCP // Fluent app (the "App"). We built the App around data minimization: we use the least data needed to provide the service, and we never sell personal data.

## 1. Scope
This policy covers data we process through the App on Shopify. It applies to Merchants who install the App and to the limited customer data that passes through the App while providing our service.

## 2. Data we access and why

**Merchant & store data.** When you install the App, we access your store's product catalog and related metadata (product titles, descriptions, variants, prices, barcodes, images, inventory, and product/sales-channel data). We use this to:
- find or generate GTIN identity and map products to GPC categories,
- create AI-generated product attributes (enrichment),
- build agent-readiness diagnostics and a supplemental product feed.

**Protected customer data (minimal).** To attribute orders that originate from AI shopping agents, the App accesses two pieces of customer data from your orders:
- **Order email** — used only to deduplicate and correlate orders. It is **hashed with SHA-256 (one-way) immediately on receipt**; we store only the hash, never the raw email.
- **Buyer IP address** — used only to help distinguish agent traffic. It is **truncated to a /24 network block immediately on receipt**; we store only the truncated value, never the full IP.

We do **not** access customer names, phone numbers, or addresses, and we do not use any data for advertising, profiling, or resale.

## 3. Google Merchant Center data (optional connection)

**UCP Fluent's use of Google Merchant Center data.** When you connect your Google Merchant Center account, UCP Fluent accesses your Merchant Center product and data-source information solely to verify feed status, manage the supplemental data source we provide, and deliver the enrichment and diagnostics features you signed up for. UCP Fluent's use of information received from Google APIs adheres to the [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy), including the Limited Use requirements. Specifically: we use this data only to provide and improve these features; we do not transfer or sell it to third parties; we do not use it for advertising; and we do not allow humans to read it except with your consent, for security purposes, to comply with applicable law, or where necessary for internal operations in compliance with the Limited Use requirements.

You can revoke the App's access to your Google account at any time at [myaccount.google.com/permissions](https://myaccount.google.com/permissions); upon revocation or uninstall we delete the stored Google tokens and connection data.

## 4. How we use data
We use the data above solely to provide the App's features — product identity, enrichment, agent-readiness monitoring, and attribution reporting shown in your dashboard. We do not sell personal data and do not share it except with the subprocessors listed below.

## 5. Data minimization & security
- Customer email is SHA-256 hashed and buyer IP is /24-truncated immediately on receipt; raw values are never stored.
- Data is encrypted in transit (TLS 1.2+) and at rest using the controls of our infrastructure provider, Google Cloud Platform.
- Access is limited to the App's automated processing pipeline and a small number of authorized personnel.
- We perform regular internal security reviews. We do not currently hold third-party certifications such as SOC 2 or ISO.

## 6. Subprocessors
- **Google Cloud Platform** — hosting, databases, and storage (all data).
- **Google Vertex AI** — generating product-attribute enrichment. Only **product/catalog data** is sent; **customer personal data is never sent to enrichment providers.**
- **Barcode Lookup / OpenFoodFacts** — looking up existing product GTINs. Only **product identifiers** are sent; no customer data.
- **Shopify** — the platform on which the App runs.

## 7. Retention
We do not store raw customer personal data — the only customer-derived values we keep are a one-way **SHA-256 hash of the order email** and a **/24-truncated IP address**, used solely for attribution (pseudonymized). We retain product/catalog data for as long as the App is installed by your store. Pseudonymized attribution records (the hashed email and truncated IP described above) are retained for up to **24 months**, after which they are automatically purged. When you uninstall the App we stop processing your store's data; on a `shop/redact` request we delete your store's data, and we honor `customers/redact` requests, within Shopify's 30-day compliance window (see Section 8).

## 8. Deletion & data-subject rights
We honor Shopify's mandatory privacy webhooks:
- **`customers/redact`** — we delete or anonymize records associated with that customer.
- **`shop/redact`** — we delete your store's data (typically within 30 days of the request or uninstall).
- **`customers/data_request`** — we provide the data we hold associated with a customer, where applicable.

Depending on your location, you and your customers may have rights under the GDPR, CCPA, or similar laws (access, correction, deletion, objection). Contact us to exercise these rights.

## 9. International transfers
The App runs on infrastructure that may process data outside your country, including in the United States and the European Union. We rely on appropriate safeguards for such transfers.

## 10. Children's data
The App is a business tool and is not directed to children.

## 11. Changes
We may update this policy. Material changes will be reflected by updating the "Last updated" date above.

## 12. Contact
**Aurina AI LLC** d.b.a. UCP // Fluent
Email: toma@ucpfluent.com
Registered address: Didgori Street 23, Tabakhmela, Tbilisi, Georgia
