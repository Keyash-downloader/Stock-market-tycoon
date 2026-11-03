# Stock Market Tycoon

A playable mobile-first virtual stock-market career simulation inspired by the broad menu/progression structure in your screenshots. It uses original game text, fictional listed companies and simulated prices.

## Included now
- Main menu and 3 local save slots
- Trader creation
- Home dashboard, career level, XP and weekly progression
- Virtual stock exchange with fictional US and Indian listings
- Buy/sell shares, cash balance and portfolio valuation
- Activities, missions, rewards, news, bank, contacts and awards
- Profile and settings, local save/load
- Mobile-first dark/gold interface

## Run as a web preview
Install Node.js, then:
```bash
npm install
npm run start
```
Open the local Vite URL on your phone or computer.

## Build Android project
You need Node.js and Android Studio / Android SDK:
```bash
npm install
npm run build
npx cap add android
npx cap sync android
npx cap open android
```
In Android Studio, wait for Gradle sync, then use **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
The generated APK is a debug build unless you create and use your own signing key.

## Important
This is a virtual educational game. It does not connect to brokers, execute real trades, provide investment recommendations, or use live market prices. All company names/prices in the prototype are fictional game data. Save slots are stored locally on the device/browser; clearing app data can erase them.

The UI is an original implementation based on high-level ideas in the supplied reference screenshots, not a copy of the original app's assets or code.

## Build APK using only your Android phone (cloud build)
A GitHub Actions workflow is included at `.github/workflows/android.yml`. Upload the project files to a GitHub repository (keep the `.github/workflows` folder), then open the repository's **Actions** tab, select **Build Android APK**, and tap **Run workflow**. When the run completes, open it and download the `Stock-Market-Tycoon-debug-apk` artifact. GitHub may require you to use the browser in Desktop site mode. This creates an unsigned-for-release debug APK for testing; it is not a Play Store release build.
