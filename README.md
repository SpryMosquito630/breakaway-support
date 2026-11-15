# Breakaway support

Public support and privacy pages for the Breakaway iOS app. This repository contains only static website content. It contains no application source, user data, or credentials.

- Support: https://sprymosquito630.github.io/breakaway-support/
- Privacy policy: https://sprymosquito630.github.io/breakaway-support/privacy.html
- Support channel: https://github.com/SpryMosquito630/breakaway-support/issues

GitHub Pages serves the root of `main`. No build tools, JavaScript, external fonts, cookies, or analytics are added by this website. GitHub operates the hosting and issue tracker under its own privacy statement.

Before changing the privacy policy, verify the behavior of the public production app, including feature gates and network services. Do not publish personal information in this repository or its issues.


## Hosted-analysis disclosure release check

The November 15, 2026 privacy update is conditional: the standard public build remains local, while builds that offer hosted Analyze disclose Google Cloud processing, sampled still images sent to Gemini, anonymous Firebase identity/App Attest, and separate retention periods. This website change does not enable uploads or certify the feature for release.

Before allowing hosted uploads in a distributed build:

- Review and merge the disclosure PR, then verify the live Pages URL displays the revised policy and the deployed Pages commit matches the reviewed commit.
- Match the in-app notice before clip selection/upload to the hosted path: selected video to Google Cloud; MediaPipe body tracking there; up to 40 downscaled timestamped stills to Gemini for subjective coaching estimates. Do not describe hosted processing as local or as an analysis computer on the user's network.
- Confirm the released build, provider configuration, Firestore expiry policies, anonymous-account cleanup, and actual data flows match this page. Recheck the 24-hour result, 48-hour request-record, and seven-day usage expiry settings. Firestore physical deletion is asynchronous; provider records have separate retention.
- Review the App Store privacy disclosures for the actual distributed build, including uploaded videos, derived results, anonymous identifiers, diagnostics/operational data, and third-party processing. This page is not a substitute for App Store disclosures.
- Verify signed-device identity/App Attest, retry/expiry behavior, permissions, and the exact user-facing upload action before enabling general use.

No video uploads, provider generation calls, or new anonymous accounts are needed to review this static disclosure change. Do not put clips, credentials, user identifiers, or private support requests into this public repository.
