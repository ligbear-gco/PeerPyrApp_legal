---
layout: default
title: Pyramid Privacy Policy
permalink: /privacy-policy/
---

# Pyramid Privacy Policy

**Effective date:** 29 October 2026<br>
**App:** Pyramid (`com.peerpyr.pyramid`)  
**Release covered:** 1.5<br>
**Developer:** **GCO-SYSTECH-INC**  
**Privacy contact:** [Privacy Contact Form](https://gco-systech.com/#contact)

This Privacy Policy explains how Pyramid handles information when you use the app. It applies to the Android app and its advertising, multiplayer and optional purchase-verification services. GCO-SYSTECH-INC is responsible for the developer-controlled processing described here. This policy remains publicly available at the URL shown in the app and in the Google Play store listing.

## What Pyramid is

Pyramid is a room-code, peer-to-peer card game. A host creates a randomly generated 10-character room code and shares it privately with friends. Players connect using PeerJS/WebRTC. The host’s device is authoritative for that game and sends the game state directly to joined players; Pyramid does not operate an account system or a game-data backend.

Treat a room code as a private bearer credential: anyone who obtains it may attempt to join the room. Do not post a room code publicly or include personal information in your display name.

## Information used for multiplayer play

To provide a game room, the app processes the following information:

| Information | Why it is used and who receives it | Retention by the developer |
| --- | --- | --- |
| Display name (up to 20 letters, numbers, or underscores) | Identifies a player to the other players in the same room. It is sent to the host and shown to room participants. | Not collected or stored by the developer. It exists in the devices’ in-memory game session and is discarded when the room/app session ends. |
| Room code and temporary player/session token | Connects a player to the intended room and supports reconnection during that session. The room code is shared with the PeerJS connection service and room participants as needed to establish the connection. | Not collected or stored by the developer. The app keeps it only for the live session. |
| Game actions and game state (for example, card visibility and revealed cards) | Lets the host run the game and lets room participants see the agreed game state. It is transmitted to the room participants. | Not collected or stored by the developer. It is held in memory for the live game. |
| Network information needed to connect | PeerJS/WebRTC and the network providers process connection-related information, such as IP address, to establish and maintain a connection. | The developer does not receive or retain it. Those providers’ own terms and privacy notices govern their processing. |

The developer does not intentionally use player names, room codes, cards, or game actions for advertising, profiling, analytics, sale, or marketing. Other players can see the display name and game activity you choose to share in the room. Do not use another person’s personal information as your display name.

## Advertising and consent choices

Pyramid uses Google AdMob to show an anchored banner in menu/lobby screens and an interstitial when a new game session begins. Ads are not required to play if an ad request or display fails.

Google’s Mobile Ads SDK may automatically collect and share the device IP address (which may estimate general location), ad/app interactions such as app launches, taps, and video views, diagnostic information such as app/SDK performance, and device or account identifiers including Android advertising ID and App Set ID. Google uses this information for advertising, analytics, and fraud prevention. Google describes its current Android SDK disclosure at [Google Play data disclosure](https://developers.google.com/admob/android/privacy/play-data-disclosure) and its broader practices in the [Google Privacy Policy](https://policies.google.com/privacy).

At launch, Pyramid requests current consent information through Google’s User Messaging Platform (UMP). When Google requires a consent form, it is shown before the app requests ads. The app requests ads only when the UMP flow reports that ads may be requested. From the main menu, open **Settings**, then **Privacy choices** to revisit Google's available choices, or **Privacy policy** to read this policy. The form, available choices, ad availability, and any personalization are determined by your region, device settings, and Google’s configured privacy message. You can also reset or delete your Android advertising ID in Android settings where that control is available.

The developer does not sell player data. Advertising data is handled by Google/AdMob and any ad technology enabled in the AdMob account. Do not enable AdMob mediation or other ad SDKs without first updating this policy and the Play Data safety declaration.

## Information Pyramid does not collect for itself

Pyramid has no application accounts, passwords, chat, user-generated uploads, developer-run analytics, customer database, or persistent game database. It offers optional consumable Superpoint purchases through Google Play, as described below. The app and its verifier do not receive card details or Google account identity. They do not ask for precise location, contacts, calendar, photos, videos, audio, files, SMS/call logs, health data, government identifiers, browsing history, biometric data, or sensitive personal characteristics.

This statement does not limit the data that Google/AdMob or the PeerJS/WebRTC connection providers may process to provide their services, as described above and in their own notices.

## Optional Superpoint purchases

Google Play handles purchase confirmation, available payment methods, payment/account information, transaction records and merchant payouts. Purchases are optional: you can play without buying anything. No separate Pyramid account is created; purchases use your Google Play account and its available payment methods. Google processes and retains its payment records under its own notices and applicable obligations; see [Google Payments Privacy Notice](https://payments.google.com/payments/apis-secure/get_legal_document?ldo=0&ldt=privacynotice) and the [Google Privacy Policy](https://policies.google.com/privacy).

A dedicated HTTPS verifier temporarily receives a Google Play purchase token and random identifiers for the current game, payer and recipient, to check and consume the purchase with Google. A one-way hash of the checkout binding is attached to the Play purchase. Display names, room codes, reconnect tokens, card values, card details and Google account identity are not sent to the verifier. The verifier creates no customer profile or purchase database and logs no request bodies, purchase tokens or provider errors. Hosting/network providers may process connection metadata under their own retention policies.

For release 1.5, purchase verification uses **Supabase Edge Functions**, with Supabase acting as a hosting processor for the developer. This does not create a Supabase account for players or store purchases in a Supabase database. The gateway necessarily receives connection information such as IP address, request time, endpoint, response status and network/device request metadata for routing, operation and security. Infrastructure logs may be retained even though our function does not log purchases. Supabase currently lists one-day API/database log retention on its Free plan; that dashboard retention period is not a promise that every security, backup or legally required record is erased after one day. See [Supabase's data processing addendum](https://supabase.com/legal/dpa) and [privacy notice](https://supabase.com/privacy). If the deployed hosting provider or its data practices change, this policy will be updated accordingly.

The payer sends only a signed, game-bound receipt to the Host. The Host holds redeemed receipt hashes in memory for that game to prevent duplicate gifts. Retry information stays in memory only. Gifts apply to the live game and cannot be restored after that game/process closes. If a completed payment cannot reach a closed game, use Google Play order history and the support contact below to request assistance/refund under applicable rules. Google Play transaction records and any correspondence or records required to resolve support/refunds are separate from the app's temporary game state.

Before checkout, the app requests product/price information from Google Play and public configuration/availability information from the verifier. Opening the gift dialog may therefore cause network requests even if you do not buy a gift. A purchase token and the game/payer/recipient binding are sent for verification only when processing a purchase or retrying it. Operational startup diagnostics identify fixed configuration steps; they do not include private keys or purchase-token values.

## Sharing and retention

The developer has no server storing multiplayer state. The purchase verifier receives only the temporary purchase information described above. The app shares the display name and gameplay data with players in the same room solely to provide multiplayer play. It uses PeerJS/WebRTC connection infrastructure, Google/AdMob ads and consent controls, and Google Play payments.

The developer maintains no multiplayer, advertising or purchase database. Verification request data is processed in function memory for the request; live game information and receipt deduplication data are discarded from the app when the game/room ends or the app is closed, subject to normal device and operating-system behavior. Google, Supabase, PeerJS, your network provider, and other players may retain information as described above and under their applicable policies and legal obligations. A request concerning developer-controlled data processed by a service provider can be made through the privacy contact; records independently controlled by another party must be addressed to that party.

Because Pyramid has no account and the developer stores no user profile, there is no account or developer-held game record to delete. For questions or a request concerning data the developer may receive through support correspondence, contact the privacy address above. For Google-controlled advertising data, use Google’s privacy controls and contact channels.

If you contact support, we receive what you send, such as your contact details, message and a Google Play order reference needed to investigate a refund. We use it to answer the request and keep it only as needed for that request, disputes, fraud prevention or applicable record-keeping obligations. Do not send card details, purchase tokens, room codes or service credentials. A support request does not create an app account.

## Processing purposes and international transfers

Where applicable data-protection law requires a legal basis, we process necessary gameplay and requested purchase-verification data to provide the service you request; security and abuse-prevention data for our legitimate interest in protecting the service; and legally required records to meet legal obligations. Advertising consent is requested where required, and available choices can be revisited as described above. Withdrawing consent does not affect processing already lawfully performed.

Google, Supabase and networking providers may process data in countries other than your own. An EU project location alone does not guarantee that all edge routing, support or provider processing remains in the EU. Where required, transfers through our processors are subject to applicable safeguards, such as contractual protections described in their data-processing terms. Contact us for questions about developer-controlled processing or applicable safeguards.

## Children and age treatment

Pyramid is a general-audience multiplayer card game intended for users **13 and older** and is not directed to children under 13 (or the minimum age requiring parental consent where they live). The app has no age gate and the developer does not knowingly collect personal information from children. Because it displays ads, offers optional purchases and allows a player-chosen name to be shared with a room, parents and guardians should supervise a minor’s use, configure Google Play purchase authentication/parental controls and keep room codes private.

If you believe a child has provided personal information to the developer through a support request, contact the privacy address above so it can be deleted where applicable.

## Security

Pyramid uses HTTPS/WSS-compatible connection services and WebRTC for gameplay connections. The Android app disables cleartext traffic and device backup for app data, uses a cryptographically secure random room-code generator, validates game messages at the host, and does not expose a developer-run database. No internet service is risk-free: protect your room code, choose a non-identifying display name, and leave any room you do not trust.

## Your rights and choices

Depending on your location, you may have rights to request access, correction, deletion, restriction, objection, or a copy of personal information controlled by the developer. Contact the privacy address above. The developer will respond as required by applicable law. Requests about Google advertising data or data controlled by another player/provider may need to be directed to that controller.

You may also complain to your local data-protection authority where applicable. We may request information reasonably necessary to verify a request, but do not require an app account or payment-card details to exercise these rights.

## Changes to this policy

We will post changes on this page and update the effective date at the top before or when they take effect. For material changes, we will also provide an in-app notice or other notice required by applicable law. Continued use after the effective date is subject to the updated policy, where permitted by law.

## Contact

For privacy questions or requests, here is our [Privacy Contact Form](https://gco-systech.com/#contact), please include “Pyramid Privacy” in the subject line.
