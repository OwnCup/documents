# Cookie, Local Storage and Web Technologies Policy

**Version 2.11-PUSH-EN.**  
**Publication and effective date: 1 September 2026.**

## 1. Scope

This Policy applies to two distinct OwnCup web resources:

1. the OwnCup marketing website – the domain on which this Policy is published;
2. the **app.owncup.eu** web application.

The resources have different origins. Cookies, localStorage and IndexedDB belonging to one resource are not automatically accessible to the other. The technologies and settings are therefore described separately below.

The native iOS and Android applications do not use browser cookies. Their local storage, permissions and SDKs are described in the **Privacy Notice**.

## 2. Operator

The operator of the resources and controller of the related personal data is KICO GLOBAL EOOD. Its details and contact information are set out in the **Legal Notice**.

## 3. OwnCup marketing website

### 3.1. Current configuration

- the DM Sans and DM Serif Display fonts are loaded from the OwnCup domain; no connection to Google Fonts is established;
- advertising pixels and marketing cookies are not used;
- Google Analytics 4 is the only optional web technology and may be loaded only after consent to analytics;
- before consent, the browser does not send requests to Google Analytics or Google Tag Manager;
- contact forms send the data entered by the user only after the submit button is clicked and do not set analytics or marketing cookies.

### 3.2. Marketing-website technology register

| Technology | Provider | Purpose | Duration | Category |
|---|---|---|---|---|
| `owncup-consent-v5` in localStorage | OwnCup | Store the required category, analytics choice, interface and document version, language, storage and expiry dates, source of the choice and a random record identifier | 6 months, until withdrawal or a material change | Strictly necessary for storing the privacy choice |
| `_ga` | Google Analytics 4 / Google Ireland Limited | Distinguish browsers for aggregated website statistics | Up to 60 days after being set or updated, subject to browser restrictions | Analytics, only after consent |
| `_ga_<container-id>` | Google Analytics 4 / Google Ireland Limited | Store the state of the analytics session | Up to 60 days after being set or updated, subject to browser restrictions | Analytics, only after consent |

Google Signals, advertising personalisation and transmission to GA4 of OwnCup’s own Account identifier, name or email address are disabled. If GA4 is not technically enabled in a particular build of the marketing website, the analytics choice is stored but does not trigger external requests.

## 4. The app.owncup.eu web application

### 4.1. Separate configuration

`app.owncup.eu` does not receive or use the marketing website’s `owncup-consent-v5` record. The web application uses its own technical storage for start-up, login, security and retention of the state of requested features.

`app.owncup.eu` loads the Google Maps JavaScript library only after the user opens the map or requests the nearby venues feature. Before that, the browser does not send a technical request to Google Maps. The device’s precise location is not transmitted without separate system permission and use of the feature for which it is required.

Flutter CanvasKit, which is needed to render the interface, is hosted on an OwnCup resource and is not loaded from Google’s infrastructure.

### 4.2. Web-application technology register

| Technology | Provider | Purpose and main data | Duration / condition | Category |
|---|---|---|---|---|
| Firebase Authentication storage in IndexedDB or localStorage | Google Firebase on OwnCup’s behalf | Secure login, session tokens and retention of Account state | Until logout, Account deletion or technical expiry | Strictly necessary for login |
| Google Maps JavaScript API | Google Ireland Limited and associated providers | Loading of the mapping library; IP address and technical request data; location only with separate permission | Only after the map is opened or nearby venues are requested; data and cache according to browser and Google settings | Functional external technology requested by the user |
| Flutter CanvasKit | OwnCup | Rendering of the web-application interface; runtime components | When the web version starts; cache according to browser settings | Strictly necessary technical web-application technology |

The application’s technical keys may have dynamic names. Their purpose is limited to application start-up, security, authentication and retention of the state of the feature selected by the user.

## 5. Native applications

Push tokens, Firebase Installation ID, secure session storage, camera, notification and location permissions, and Firebase Cloud Messaging and Apple Push Notification Service are not cookies. They are described by purpose and resource in sections 3 and 10 of the Privacy Notice. Marketing push messages are permitted only after the relevant category is selected separately in the application; the device's system permission alone is not marketing consent.

Firebase Remote Config, if used by the installed build, is also not a cookie. It is used only for a separately documented technical purpose and is not used to form a marketing audience. A parameter needed exclusively for a marketing function is not fetched before that function is activated.

## 6. Consent on the marketing website

Strictly necessary storage is used without separate consent only to store the privacy choice, provide security and perform a function expressly requested by the user.

For analytics, the marketing website provides equivalent options:

- “Accept all”;
- “Reject optional”;
- “Customise”.

Silence, scrolling, continued use and a pre-selected analytics option do not constitute consent. Refusal of analytics does not restrict the website’s core functions.

## 7. Choice period and withdrawal

The marketing-website choice is stored for 6 months. The user may select the persistent **“Settings”** button at any time, change the decision or withdraw consent. Following withdrawal, accessible `_ga` and `_ga_<container-id>` cookies are deleted and no new analytics requests are sent.

Clearing localStorage or cookies in the browser may cause the panel to be displayed again. Blocking `app.owncup.eu` technical storage may prevent login or operation of the web application.

## 8. Third-party providers

Google processes technical requests for Google Analytics, Google Maps and Firebase in accordance with the applicable contractual terms and the [Google Privacy Policy](https://policies.google.com/privacy?hl=en). The roles, data categories and international transfers are also described in the **Privacy Notice** and the **Service Providers and Data Recipients Register**.

## 9. Changes and contact details

When the web technologies actually in use change, OwnCup updates this register and, where required, requests a new choice before activating an optional technology. Questions should be sent to **privacy@owncup.eu**.
