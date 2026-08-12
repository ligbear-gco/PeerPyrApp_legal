# Pyramid launch publishing checklist

This checklist closes the items that require account-owner action and cannot be completed reliably from source code alone.

## Required before the public policy is valid

- [ ] Replace the developer-name placeholder in `privacy-policy.md` and `terms-of-use.md` with the exact legal entity or individual displayed in Google Play.
- [ ] Replace each contact-email placeholder with a monitored privacy/support inbox.
- [ ] Confirm the effective date is correct and commit the completed documents.
- [ ] In GitHub repository settings, enable Pages from `main` and confirm this exact logged-out HTTPS URL opens: `https://ligbear-gco.github.io/PeerPyrApp_legal/privacy-policy/`.
- [ ] Do not use the GitHub `blob` URL, a local file, or an unauthenticated preview as the Play policy URL.

## Required app integration

- [ ] Set `VITE_PRIVACY_POLICY_URL=https://ligbear-gco.github.io/PeerPyrApp_legal/privacy-policy/` in the production build environment.
- [ ] Build, install, and confirm the app’s **Privacy policy** link opens that URL on a real device.
- [ ] Confirm **Privacy choices** opens Google’s UMP privacy options when UMP requires/provides them.
- [ ] Confirm production has `VITE_ADMOB_USE_TEST_ADS=false`, no test-device list, real AdMob IDs, and no demo ID.

## Required Play Console completion

- [ ] Enter the exact policy URL in the designated privacy-policy field.
- [ ] Declare **contains ads: Yes**.
- [ ] Complete App content, reviewer app access, target audience (13+ only), IARC content rating, and Data safety using `play-console-declarations.md` and the current Console wording.
- [ ] Inspect the final `.aab` and all enabled AdMob mediation/ad sources before submitting; update the declaration and policy for any difference.
- [ ] Configure AdMob ad-content controls appropriate for the IARC result and the 13+ audience.
- [ ] Revisit the documents and Data safety declaration before every release that changes data practices, SDKs, ads, permissions, audience, or developer identity.
