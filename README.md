# RentPro — GitHub APK Builder

This repository packages the RentPro HTML app as an Android APK using Capacitor and GitHub Actions.

## Build your APK on GitHub

1. Create a new **public or private** GitHub repository (for example, `RentPro`).
2. Upload all files and folders from this project. Make sure `.github/workflows/build-apk.yml` is included.
3. Open the repository's **Actions** tab.
4. Select **Build RentPro APK** and click **Run workflow**. (A push to `main` also starts a build.)
5. Wait for the workflow to finish successfully.
6. Open the completed workflow run and download the **RentPro-Android-APK** artifact.
7. Extract the downloaded ZIP. The APK inside is `app-debug.apk`. Transfer it to your Android phone and install it. Android may ask you to allow installation from that source.

## App data

RentPro stores records in the app's local browser storage on that device. Uninstalling the app or clearing its storage can erase records. Use **Reports & backup → Export backup** regularly and keep the JSON backup somewhere safe.

## Package details

- App name: RentPro
- Android application ID: `com.rentpro.broker`
- Build type: Debug APK (suitable for testing / direct installation)

For a Play Store release, create a signed release build with a private keystore. Do not commit signing keys or passwords to GitHub.
