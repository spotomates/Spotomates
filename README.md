# SpotoMates website

Static HTML and CSS. Serve the repository root; directory URLs must resolve to their `index.html`. There is no package install or build step.

## Cozy Express pages

- `/cozy-express/privacy/`
- `/cozy-express/support/`
- `/cozy-express/friends-rules/`

Contact: `spots@spotomates.com`. No postal address is included. The pages use local styles and no JavaScript, analytics, cookies or third-party font requests.

These files were prepared locally on November 3, 2026. They have not been published by this task. The public copy is written for the full released iPad game, as requested by the owner; it must be published with the matching release behavior, not the older internal-test service. The website's current deployment mechanism is not configured in this checkout.

**Support correction, November 9, 2026 — publication pending.** `cozy-express/support/index.html` now explains that ended paid access locks premium creations and extra capacity, preserves original saves for valid paid access to return, and keeps free play and eligible received gifts available. This matches the game's `Docs/PREMIUM_SPEC.md`. The live support URL returned HTTP 200 on November 9 but still promised that existing creations stay available. Publish the corrected support file through the existing host, then verify the public refund section and updated date. This correction has not been deployed from this checkout.

## Before using the URLs in App Store Connect

1. Publish all three directories and `cozy-express/info.css` on the existing `spotomates.com` host. Verify each HTTPS URL opens without a login, including direct visits and links between pages.
2. Deploy the matching Friends backend through migration 011 and use a player containing the privacy, age, moderation and agreement changes. The existing service recorded in the game repository is older; do not present the new retention/deletion behavior as current until that deployment matches.
3. Verify the launch copy against StoreKit, Restore Purchases, the final Full Game contents and Family Sharing before publication. Those purchase features are described as release features by the owner’s explicit request, but are still future work in the game checkout. Prices remain store-provided; no fixed amount is advertised.
4. Verify the email is monitored, report notices reach the moderator, and deletion/support requests can be handled. Confirm the host's log and backup windows and update privacy text with the verified details. Confirm distribution-build network behavior before asserting that diagnostics are absent.
5. Set App Store Connect's Privacy Policy URL to `https://spotomates.com/cozy-express/privacy/` and Support URL to `https://spotomates.com/cozy-express/support/`. These same routes are in the game's `CozyLegalInfo` constants. The Friends rules are version 1, dated November 3, 2026; material changes must also bump the in-game agreement version.

The pages are not a statement that App Review has approved the app. Review the actual release against Apple's current requirements. Reference checks used [App Review Guidelines](https://developer.apple.com/app-store/review/guidelines/) §§1.2, 1.5 and 5.1.1, [account deletion guidance](https://developer.apple.com/support/offering-account-deletion-in-your-app/), [purchase restoration](https://support.apple.com/en-us/108096), and [refund guidance](https://support.apple.com/en-us/118223). The game's launch plan retains the separate audience and regional release questions.
