# Build the Android APK

This project includes a GitHub Actions workflow that builds the APK automatically.

## Easiest method

1. Create a GitHub account if you do not already have one.
2. Create a new repository, for example `character-reference-studio`.
3. Upload the contents of this project ZIP to that repository.
4. Open the repository's **Actions** tab.
5. Select **Build Android APK**.
6. Run the workflow if it did not start automatically.
7. When it finishes, open the workflow run and download the artifact named:
   `Character-Reference-Studio-APK`
8. The downloaded ZIP contains `app-debug.apk`.
9. Transfer the APK to your Android phone and install it.

GitHub's hosted Linux runners can run Android builds, and Capacitor supports producing an APK from the native Android project.

### Important
This is a debug APK intended for personal installation/testing. A signed release APK/AAB for Play Store distribution is a separate step.

For local/native builds, current Capacitor Android setup requires Android Studio and an Android SDK. Node 22+ is required by current Capacitor tooling.
