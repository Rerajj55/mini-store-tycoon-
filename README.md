# Mini Store Tycoon — Android Monetized Test Project

This project wraps the playable HTML game in a native Android app and adds:
- Google Mobile Ads test banner
- Google Mobile Ads test interstitial hook
- Google Mobile Ads test rewarded ad (+₱500)
- Google Play Billing one-time product: `remove_ads`
- Local game save through the HTML game
- Portrait Android UI

## Open/build
1. Install Android Studio (2026.x recommended).
2. Open this folder as an existing Gradle project.
3. Let Gradle sync.
4. Run the `app` configuration on an emulator or Android phone.

## Test ads
The project uses Google's official demo ad IDs. These are safe for development/testing. Replace them with your own IDs before publishing.

## Remove Ads purchase
The product ID is `remove_ads`.
To test the actual Google Play purchase flow, create a one-time in-app product with that exact ID in Play Console and publish the app to an internal/closed test track. Add your Google account as a license tester. Test purchases are not charged to license testers.

## Important for release
- Replace the sample AdMob App ID and ad unit IDs.
- Create `remove_ads` as a one-time in-app product in Play Console.
- Use a proper privacy/consent flow as required for your audience and regions.
- Verify purchases securely and handle entitlement server-side for a production monetized app.
- Create your own signed release keystore/AAB.
