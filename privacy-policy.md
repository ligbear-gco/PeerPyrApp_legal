---
layout: default
title: Pyramid Privacy Policy
permalink: /privacy-policy/
---

# Pyramid Privacy Policy

**Effective date:** 12 August 2026  
**App:** Pyramid (`com.peerpyr.pyramid`)  
**Developer:** **GCO-SYSTECH-INC**  
**Privacy contact:** [Privacy Contact Form](https://gco-systech.com/#contact)

This Privacy Policy explains how Pyramid handles information when you use the app. It applies to the Android app and its advertising and multiplayer services. This policy must remain publicly available at the URL shown in the app and in the Google Play store listing.

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

At launch, Pyramid requests current consent information through Google’s User Messaging Platform (UMP). When Google requires a consent form, it is shown before the app requests ads. The app requests ads only when the UMP flow reports that ads may be requested. You can revisit Google’s available choices from the app’s **Privacy choices** button. The form, available choices, ad availability, and any personalization are determined by your region, device settings, and Google’s configured privacy message. You can also reset or delete your Android advertising ID in Android settings where that control is available.

The developer does not sell player data. Advertising data is handled by Google/AdMob and any ad technology enabled in the AdMob account. Do not enable AdMob mediation or other ad SDKs without first updating this policy and the Play Data safety declaration.

## Information Pyramid does not collect for itself

Pyramid has no user accounts, passwords, in-app purchases, chat, user-generated uploads, developer-run analytics, or developer-run cloud database. It does not ask for or intentionally collect precise location, contacts, calendar, photos, videos, audio, files, SMS/call logs, health data, financial information, government identifiers, browsing history, biometric data, or sensitive personal characteristics. It requests only Android internet access.

This statement does not limit the data that Google/AdMob or the PeerJS/WebRTC connection providers may process to provide their services, as described above and in their own notices.

## Sharing and retention

The developer has no server that receives or stores multiplayer data. The app shares the display name and gameplay data with the players in the same room solely to provide multiplayer play. It uses PeerJS/WebRTC connection infrastructure to establish that play and Google/AdMob to provide ads and consent controls.

The developer retains no multiplayer or advertising records. Live game information is discarded from the app when the room is left or the app is closed, subject to normal device and operating-system behavior. Google, PeerJS, your network provider, and other players may retain information under their own policies and legal obligations; the developer cannot delete information they independently control.

Because Pyramid has no account and the developer stores no user profile, there is no account or developer-held game record to delete. For questions or a request concerning data the developer may receive through support correspondence, contact the privacy address above. For Google-controlled advertising data, use Google’s privacy controls and contact channels.

## Children and age treatment

Pyramid is a general-audience multiplayer card game intended for users **13 and older** and is not directed to children under 13 (or the minimum age requiring parental consent where they live). The app has no age gate and the developer does not knowingly collect personal information from children. Because it displays ads and allows a player-chosen name to be shared with a room, parents and guardians should supervise a minor’s use of the app and should not share room codes publicly.

If you believe a child has provided personal information to the developer through a support request, contact the privacy address above so it can be deleted where applicable. Do not select any Google Play target-audience age group under 13 unless the app is redesigned, its advertising setup is made Families-policy compliant, and this policy and the Play declarations are updated first.

## Security

Pyramid uses HTTPS/WSS-compatible connection services and WebRTC for gameplay connections. The Android app disables cleartext traffic and device backup for app data, uses a cryptographically secure random room-code generator, validates game messages at the host, and does not expose a developer-run database. No internet service is risk-free: protect your room code, choose a non-identifying display name, and leave any room you do not trust.

## Your rights and choices

Depending on your location, you may have rights to request access, correction, deletion, restriction, objection, or a copy of personal information controlled by the developer. Contact the privacy address above. The developer will respond as required by applicable law. Requests about Google advertising data or data controlled by another player/provider may need to be directed to that controller.

## Changes to this policy

We will post changes on this page and update the effective date at the top before or when they take effect. For material changes, we will also provide an in-app notice or other notice required by applicable law. Continued use after the effective date is subject to the updated policy, where permitted by law.

## Contact

For privacy questions or requests, here is our [Privacy Contact Form](https://gco-systech.com/#contact), please include “Pyramid Privacy” in the subject line.
