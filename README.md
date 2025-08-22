# SimpleHelloApp

This repo contains a minimal Android app written in Kotlin.

## Build an APK in Android Studio (fastest)
1. Open the project in **Android Studio**.
2. Wait for Gradle sync.
3. **Build** → **Build Bundle(s) / APK(s)** → **Build APK(s)**.
4. Grab the APK from `app/build/outputs/apk/debug/`.

## Build with GitHub Actions (no local Android Studio required)
1. Create a new GitHub repo and push these files.
2. Go to **Actions** tab and enable workflows.
3. Run the workflow **Android CI (Debug APK)** (or push to `main`).
4. When it finishes, download the artifact named **SimpleHelloApp-debug-apk**; it contains the debug APK.

> Note: The workflow will generate a Gradle Wrapper automatically if it's missing.

## Local CLI build (optional)
If you have the Android SDK + JDK 17 installed, you can also run:
```bash
./gradlew assembleDebug
```
