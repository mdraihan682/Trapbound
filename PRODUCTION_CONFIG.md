# EXTERNAL CONFIGURATION REQUIRED

## AdMob
Choose a maintained Cordova AdMob integration compatible with your final Cordova Android version. Add your real App ID and ad unit IDs in the plugin/configuration. Use Google's test ads during development. Only show interstitials at natural transitions and never as a forced death-loop.

The code's `AdManager` is intentionally an abstraction; it does not fake ad revenue.

## Google Play Billing
Create a non-consumable product for Remove Ads in Play Console (target price $0.99 USD equivalent; regional prices are controlled by Google Play). Configure a maintained Cordova purchase plugin and product ID. Verify purchase state; do not trust localStorage as proof of entitlement. Restore purchases on reinstall.

The code's `PurchaseManager` does not fake successful purchases.

## Privacy / Play Console
Complete your privacy policy, Data Safety form, content declarations, ads declaration, app signing, store listing and testing tracks before release.
