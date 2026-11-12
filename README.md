# Garage Monitor for iOS

An Expo and React Native app for browsing three vehicle profiles and displaying telemetry when a compatible gateway is configured.

## Local development

Use Node.js 22 or later. On macOS with Xcode and CocoaPods installed:

```sh
npm ci
npm run check
npm test
npm run ios
```

Without gateway settings the app opens with its empty-data UI. The build uses generated vehicle illustrations.

## iOS simulator build

GitHub Actions runs the **iOS Simulator Build** workflow on macOS. A successful run attaches the Release simulator app as an artifact. It can be installed on a booted simulator with `xcrun simctl install booted GarageMonitor.app`.
