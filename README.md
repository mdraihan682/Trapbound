# Trapbound: Fat Dash — 500 Level Cordova Game

Original mobile-first 2D surprise/trap platformer built only with HTML5 Canvas, CSS, JavaScript and Apache Cordova.

## Included
- 500 data-driven levels, 20 worlds × 25 levels
- 20 visual themes including Summer, Rain, Thunder, Winter, Ocean, Hell, Heaven, Space, Alien and more
- 25 animal trap identities
- Reusable trap framework
- Fat original player drawn with Canvas
- Touch + keyboard controls
- Landscape responsive canvas
- Local save/progression/coins/achievements
- Cosmetics shop
- Daily challenge UI
- Ad and billing abstraction points

## Important
No client-only game can be made literally "unhackable". A determined user can modify a local APK/save. This project therefore keeps the campaign offline and free, while purchase/ad entitlements are intentionally not faked. Production purchases should be verified through Google Play's supported billing flow and, for strong entitlement security, a backend.

Ads and Google Play Billing are **EXTERNAL CONFIGURATION REQUIRED**. Do not ship with test IDs as production IDs.

The 500 levels are procedurally authored into static level-data files using deterministic seeds. Each level has its own seed-derived layout, trap mix, collectible placement and theme progression; the shared engine prevents duplicated 500-function code.


## GitHub Actions APK/AAB Build

This project includes `.github/workflows/build.yml`.

After uploading the project to GitHub:
1. Push to `main` or `master`, or open **Actions → Build Android APK and AAB → Run workflow**.
2. Wait for the workflow to finish.
3. Open the completed workflow run.
4. Under **Artifacts**, download `Trapbound-Android-Builds`.

The workflow builds a debug APK and an unsigned release AAB. A production Play Store release still needs proper app signing/keystore configuration.
