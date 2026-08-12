# Pyramid — Google Play Console declaration worksheet

**Package:** `com.peerpyr.pyramid`  
**Policy URL:** [Privacy Policy](https://ligbear-gco.github.io/PeerPyrApp_legal/privacy-policy/)

## Store listing

| Field | Proposed value |
| --- | --- |
| App name | Pyramid |
| App type/category | Game; Card |
| Pricing | Free |
| Contains ads | **Yes** — AdMob banner and interstitial |
| Privacy policy | [Privacy Policy](https://ligbear-gco.github.io/PeerPyrApp_legal/privacy-policy/) |
| Developer/contact | Use the exact legal developer/business name and monitored email that replace the placeholders in the policy. |
| App access | No account or restricted access. Reviewers can create a room and join from a second device; ads depend on network/AdMob availability. |

Do not claim the app is ad-free, offline-only, or that it collects no data.

## Target audience and children

Set the app as **not designed for children**. Select only the Play age bands for **13 and older** that are available in the current Console. Do not select an under-13 age band. The app is a general-audience social card game with Google ads and room-code multiplayer, has no age gate, and is not designed for children.

If any under-13 group is selected later, stop submission and complete the Families-policy work first: age treatment, parent/guardian design, child-directed ad configuration, a Families Self-Certified Ads SDK setup, and updated policy/Data safety disclosures.

## App content

| Console topic | Proposed answer, based on the released app |
| --- | --- |
| Ads | **Yes**. Banner in menu/lobby; interstitial at a new game session/replay. |
| App access | No login credentials required. Provide the two-device room-code instructions above. |
| Target audience | 13+ only; not designed for children. |
| Privacy policy | Provide the exact policy URL above. |
| Social features | No chat, posts, public profiles, or user-generated media. Players can choose a display name and share game state with people in the same private room. Answer current Console questions from this behavior. |
| Financial features | No real-money gambling, prizes, purchases, or financial products. |
| Data deletion | No account and no developer-held profile/game data. The policy explains this and gives a contact for support correspondence. |

## Content rating (IARC)

Choose **Game** and answer the current IARC questionnaire from the implementation, not from the desired rating. The app itself has cards only: no violence, sexual content/nudity, profanity, drugs/alcohol/tobacco, horror, gambling for money, purchases, or user-generated content. It does contain third-party ads, so configure AdMob blocking/content ratings so ads and their offers are appropriate for the rating that IARC assigns. Do not pre-state a final PEGI/ESRB/IARC rating: IARC assigns it from the submitted questionnaire.

## Data safety — required baseline declaration

Answer **Yes** to “Does your app collect or share any of the required user data types?” The answer is yes because the Google Mobile Ads SDK sends data off-device, and the peer-to-peer game sends a chosen display name and game/session information to other players/connection infrastructure. All listed transmission must be reflected even though the developer runs no backend.

| Data type in Play | Why it applies | Purpose(s) to select/confirm | Collected/shared assessment |
| --- | --- | --- | --- |
| Personal info — Name | A player-selected display name is sent to the host/room participants for multiplayer play. | App functionality | Collected/transmitted off device for the feature; confirm the Console’s current recipient definition and mark sharing where required. |
| Location — Approximate location | The Ads SDK collects IP address, which Google says may estimate general location. | Advertising, analytics, fraud prevention | Google Mobile Ads SDK automatic collection/sharing. |
| App activity — App interactions | Google states the Ads SDK collects app launch, taps, and video-view interactions. | Advertising, analytics, fraud prevention | Google Mobile Ads SDK automatic collection/sharing. |
| App info and performance — Diagnostics | Google states the Ads SDK collects app/SDK performance data, including launch time, hang rate, and energy usage. | Advertising, analytics, fraud prevention | Google Mobile Ads SDK automatic collection/sharing. |
| Device or other identifiers | Google states the Ads SDK collects Android advertising ID, App Set ID, and potentially other signed-in account identifiers. | Advertising, analytics, fraud prevention | Google Mobile Ads SDK automatic collection/sharing. |
| Room code, temporary player token, gameplay state | Used to establish and run the live room; may not map to a named Play data type by itself. | App functionality | Documented in the policy. Re-check the current form definitions; do not omit a category if Play maps an element to one. |

For the form’s security questions, the Google Ads SDK documentation states its collected data is encrypted in transit. The app also uses encrypted network transport configuration. Select “all data encrypted in transit” only after testing/confirming every production endpoint and SDK. Do **not** claim a developer-held data-deletion mechanism for Google/AdMob data unless the final account setup and policy provide one; the developer has no account or backend data. Use Google’s controls for Google-controlled data.

Before submitting, inspect the final dependency report and AdMob account. Any mediation adapter, Firebase/analytics SDK, crash reporting SDK, ad format, or new permission can change these declarations.

## Evidence in the release implementation

- `@capacitor-community/admob` is initialized only on native mobile, requests UMP consent at launch, requests ads only when `canRequestAds` is true, and exposes the **Privacy choices** form.
- Production configuration uses an AdMob banner and interstitial only; no rewarded unit is implemented.
- The app has only `android.permission.INTERNET`; it has no account, sign-in, storage, location, contacts, camera, microphone, analytics, or purchase implementation.
- PeerJS uses a host-authoritative WebRTC room. Player names, codes, tokens, and game state are live-session information; the developer runs no game server/database.

## Final owner confirmations

1. Replace every `[REPLACE BEFORE PUBLISHING]` field in the policy and terms with the exact developer identity and a working email.
2. Enable GitHub Pages, test the policy URL while signed out, and set `VITE_PRIVACY_POLICY_URL` to the exact URL in the release environment.
3. In AdMob, create and publish the required UMP privacy message, verify consent and the Privacy choices entry point on an EEA/UK/Swiss test device, and set suitable ad-content controls.
4. Validate every answer in the current Console UI; Google changes its questionnaires and SDK disclosures over time.
