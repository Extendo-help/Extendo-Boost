# Extendo Boost

A starter Android app project for the Extendo Boost game launcher.

## What this starter build does

- Lists launchable apps installed on the phone.
- Lets you choose an app and open it with **BOOST & PLAY**.
- Shows battery percentage, battery temperature (when exposed by Android), available RAM, and display refresh rate.
- Provides shortcuts to Android display and system settings.
- Includes a GitHub Actions workflow that builds a debug APK and stores it as a downloadable artifact.

## Important limitations

This is a **starter version**, not a magical FPS booster. Standard Android apps cannot generally force another game's internal rendering resolution, replace its textures, disable that game's shadows/effects, or overclock CPU/GPU frequencies without privileged access. The profile picker currently records a user choice in the interface; it does not apply hidden system tweaks.

The displayed temperature is the **battery temperature**, not a direct GPU or CPU temperature. RAM figures describe system memory, not a guaranteed amount recoverable for the game. Actual FPS depends on the phone, game, temperature, and game settings.

## Build an APK on GitHub

1. Create a GitHub repository.
2. Upload the contents of this project, preserving the `.github/workflows/build.yml` path.
3. Open the repository's **Actions** tab.
4. Select **Build Extendo Boost APK** and press **Run workflow**, or push a commit to `main`/`master`.
5. Open the completed run and download the `Extendo-Boost-debug-apk` artifact.
6. Extract the downloaded ZIP and install the APK on your Android phone if you trust the source.

The generated APK is a **debug build** for testing. It is not a Play Store release.

## Project details

- Application ID: `com.extendo.boost`
- Minimum Android version: Android 6.0 (API 23)
- Compile SDK: Android 15 (API 35)
- Version: `0.1.0`
