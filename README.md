# CoreArsitek iOS WebView (Dummy Full Project)

This project is a ready-to-upload **dummy** Flutter project structured to be accepted by CI systems like Codemagic.
It includes an `ios/` folder with the minimal Xcode project files, `lib/main.dart` with a WebView using the requested URL,
and a `codemagic.yaml` to start an iOS release workflow.

**WebView URL**: https://corearsitek.id

**Important note:** This project was generated without running `flutter create` here. Codemagic usually runs `flutter pub get` and
builds the iOS project; in case Codemagic reports missing Flutter-generated build files, you may need to run `flutter create` locally
once and commit the resulting `ios/` folder, or let me know and I'll provide further fixes.

## How to use
1. Extract the zip.
2. Push to a GitHub repo.
3. Connect repo to Codemagic.
4. In Codemagic, configure iOS code signing (p12 or App Store Connect API Key).
5. Run the `ios-webview-release` workflow.