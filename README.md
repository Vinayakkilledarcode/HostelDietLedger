# Hostel Diet Ledger — Android app

WebView-wrapped diet ledger. Fully offline (fonts bundled), 7-bottle water tracker that resets daily.

## Build the APK — pick one

### A) Android Studio (Ladybug or newer, JDK 17+)
1. File → Open → select this `HostelDietLedger` folder. Gradle wrapper is included, so sync works.
2. Build → Build APK(s). Output: `app/build/outputs/apk/debug/app-debug.apk`

### B) Command line (JDK 17 + Android SDK)
```
./gradlew assembleDebug      # app/build/outputs/apk/debug/app-debug.apk
./gradlew assembleRelease    # app/build/outputs/apk/release/app-release.apk (signed)
```

### C) No setup — GitHub Actions
Push this folder to a GitHub repo. Actions → "Build APK" → download the `HostelDietLedger-apk` artifact.

Release signing uses the bundled `app/release.keystore` (password `dietledger123`) — fine for sideloading;
replace it before any Play Store upload.
