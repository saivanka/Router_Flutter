# Router_Flutter

A minimal Flutter demo of navigating between two pages. The whole app lives in the `demo/` folder: a first page with a button that pushes a second page onto the navigation stack, passing it a string.

## What it does

- **FirstPage** (`demo/lib/main.dart`): shows an app bar titled "Routing", the text "FirstPage", and a "Go to Second Page" button.
- **Navigation**: tapping the button calls `Navigator.of(context).push()` with a `MaterialPageRoute` that builds `SecondPage`, passing the string `'Hello there from the first page!'` as its `data` argument.
- **SecondPage** (`demo/lib/main.dart`): shows an app bar titled "Routing" and the text "Welcome to SecondPage".

## Tech stack

- Flutter (Dart) with Material widgets only — no third-party packages beyond the Flutter SDK and `cupertino_icons`.
- The demo project is named `demo`, version 1.0.0+1.

## How to run

```bash
cd demo
flutter pub get
flutter run
```

The demo targets the older Dart SDK range in `demo/pubspec.yaml` (`>=2.7.0 <3.0.0`), so it may need an older Flutter toolchain or SDK updates to run on a current setup.

## Project structure

```
demo/
  lib/
    main.dart      # MyApp, FirstPage and SecondPage — the entire demo
  android/         # Android project files
  ios/             # iOS project files
  test/            # Flutter test folder
  pubspec.yaml     # Project "demo", version 1.0.0+1
  README.md        # The stock Flutter template README for the demo
```

## Status

A single-commit 2021 learning demo. It demonstrates one push navigation and passing data to the next page — nothing more. The repository's only branch is `stage-v.1.0`, and there is no README inside `demo/` beyond the stock template one.
