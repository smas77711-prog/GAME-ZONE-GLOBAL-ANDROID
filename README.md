# GAME ZONE GLOBAL — Android wrapper

This is an Android WebView app that opens the existing production store at https://game-zone-store-one.vercel.app/ . It does not create a second store or duplicate the backend.

## Build an APK

1. Open this folder in Android Studio (current stable version).
2. Let Gradle sync and install Android SDK Platform 35 if prompted.
3. Select **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
4. Debug APK output: `app/build/outputs/apk/debug/app-debug.apk`.

Alternatively, push this project to a GitHub repository. The included GitHub Actions workflow builds the debug APK; run it from the Actions tab and download the artifact.

## Important notes

- Package: `com.gamezone.global`
- Minimum Android: 6.0 (API 23)
- Target SDK: 35
- Existing website login, products and vendor purchase links remain hosted by the website.
- This is a WebView wrapper, not a fully native app. Native push notifications and in-app payments are not implemented.
- Test sign-in, email confirmation, password reset, checkout/vendor links and back navigation on a real Android device before public release.
