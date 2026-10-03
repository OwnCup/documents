# Service Providers and Data Recipients Register

**Version 2.11-PUSH-EN.**  
**Publication and effective date: 1 September 2026.**

## 1. Purpose

The register lists the principal ongoing service providers and recipients that may have access to personal data to the extent necessary for the operation of OwnCup or performance of an Agreement or law. The role of a particular organisation depends on the relevant service: it may process data on OwnCup’s behalf or act as an independent recipient on a basis established by law.

The marketing website, `app.owncup.eu` and the native applications use different sets of technologies. The surface on which each is used is stated separately so that the presence of a provider in one part of the service is not understood as meaning that it is automatically used in every other part.

## 2. Principal service providers and recipients

| Provider or recipient | Surface | Purpose and main data | Principal place of processing |
|---|---|---|---|
| Vercel Inc. | marketing website `owncup.eu` | Hosting and processing under the applicable DPA, global CDN, TLS, protection against DDoS and abuse, page delivery and technical diagnostics; IP address, date and time, requested path, headers, response status and limited technical request information | Global edge infrastructure; for transfers to the United States, the EU–U.S. Data Privacy Framework for covered data while Vercel maintains a valid certification, and where that mechanism does not apply, the Standard Contractual Clauses incorporated into the DPA and necessary supplementary measures |
| Google Cloud and Firebase | `app.owncup.eu`, native applications and OwnCup back end | Authentication, application and API, file storage, technical logs, separately documented remote configuration, and delivery of service and selected marketing notifications; Account identifiers, FCM registration token, Firebase Installation ID where actually used, language, platform and minimal technical data. FID and Remote Config are not used to form a marketing audience | EU/EEA selected as the location for primary resources; certain services and support may use global infrastructure |
| Google Analytics 4 / Google Ireland Limited | marketing website, only after consent and only if GA4 is enabled in the published build | Aggregated statistics; online identifiers, browser and device information, pages visited and interaction events | Google infrastructure may involve processing outside the EEA subject to applicable safeguards |
| Google Maps Platform | `app.owncup.eu` and map features in native applications | After the map is opened or nearby venues are requested: mapping library, IP address, technical request data and, after separate permission, location for the requested feature | Google’s global infrastructure; the request may involve a transfer outside the EEA |
| Apple Push Notification Service | native iOS application | Delivery of service and selected marketing notifications; APNs device token and minimal technical delivery metadata | Apple’s global infrastructure |
| MongoDB Atlas | OwnCup back end for web and native applications | Primary database and backups; service data | Selected hosting in the EU/EEA; support may be provided from other countries |
| OwnCup email infrastructure | marketing website, Accounts, support and B2B | Contact forms, required service emails and support responses; email address and message content | Estonia, EEA |
| Apple App Store and Google Play | distribution of native applications | Store-account, download and payment data received by the relevant store as an independent controller under its own terms | As stated in the relevant store’s notices |
| Client whose programme the Guest participates in or whose campaign the Guest receives | programme and Client-initiated campaign | In the loyalty-programme interface, as a joint controller, the Client has access to the displayed or generated name, time, offer/transaction type, reward, status and limited history for that Programme only. For a push campaign, the Client supplies the Material, Locations and period but does not receive the Recipients' personal and technical data listed in section 10.2 of the **Business Client Terms of Service** | The relevant Client’s active market; access through OwnCup’s secure interface |
| Bank and accounting providers | B2B relationship | Payments, invoices and mandatory accounting; business-client and payment data | Bulgaria / EEA |

## 3. International transfers and updates

For transfers outside the EEA, OwnCup uses an applicable adequacy decision, the EU–U.S. Data Privacy Framework for a covered certified recipient, or Standard Contractual Clauses and the necessary supplementary measures.

The register does not include providers that are not intended to receive user data from the service. The register is updated where there is a material change to an ongoing recipient, purpose or surface of use. Questions: **privacy@owncup.eu**.

Flutter CanvasKit is hosted on an OwnCup resource and is therefore not listed as a separate external data recipient.
