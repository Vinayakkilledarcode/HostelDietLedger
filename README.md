# Hostel Diet Ledger

A personal project I built to keep my hostel-mess diet on track. The mess menu rotates on a two-week cycle, so I turned it into an offline Android app: every meal has calories and protein, every day has a total against my target, and a bottle tracker keeps me honest about water.

## Features
- Two-week rotating menu (Week 1 / Week 2, Sunday to Saturday)
- Per-meal and per-day calorie and protein totals, with how far under the calorie target and over the protein floor each day lands
- Daily water tracker (7 bottles, about 3.6 L) that resets automatically each day
- My standing "running rules" for the mess (one fried item a day, small rice portions, water before meals)
- Light and dark theme, follows the phone
- Fully offline: fonts and data are bundled, no account, no tracking

## Tech
- Android WebView shell (Java), single-page app in plain HTML, CSS and JavaScript (`app/src/main/assets/index.html`)
- Data stored on-device with `localStorage`
- Gradle 8.7, Android Gradle Plugin 8.3.2, min SDK 21, target SDK 34
- GitHub Actions builds the APK on every push

## Get the APK
Push to `main`, open the **Actions** tab, open the latest **Build APK** run, and download the `HostelDietLedger-apk` artifact (`app-debug.apk` and a signed `app-release.apk`).

Or build locally in Android Studio: open the folder, sync, then Build > Build APK(s).

## Notes
Calorie and protein numbers are estimates from standard Indian-food references, not lab values. The app is a personal planning aid, not medical or nutritional advice.

## Author
Vinayak Killedar (VK) - [github.com/Vinayakkilledarcode](https://github.com/Vinayakkilledarcode)
