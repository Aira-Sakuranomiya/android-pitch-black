# Pitch Black

A minimal Android app that displays a solid black screen in immersive mode,
with the status bar and navigation bar hidden. Supports Android 6.0 and later.
No controls, third-party runtime dependencies, or permission requests.

Open the project in Android Studio, or build and install it from the command line:

```sh
./gradlew assembleDebug
adb install -r app/build/outputs/apk/debug/app-debug.apk
```

The Gradle daemon uses JDK 25, as configured in `gradle/gradle-daemon-jvm.properties`.
Compile SDK: Android 37.2. Target API: 36. Java source compatibility: 17.
The APK is generated at `app/build/outputs/apk/debug/app-debug.apk`.
Application ID: `cafe.aira.pitchblack`.

The app name follows the system language: Chinese uses the localized name;
all other languages default to "Pitch Black".

Swipe from a screen edge to reveal the system bars temporarily; they hide again
automatically. Use the system Back or Home gesture to leave the app.
