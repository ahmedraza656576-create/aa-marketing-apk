# A.A Marketing — Android APK project

This repository packages the supplied React app as an Android application using Vite and Capacitor.

## Files

- `src/App.jsx` — your original React app code (keep this filename).
- `src/main.jsx` — React entry point.
- `index.html` — web app shell.
- `public/logo.png` — supplied A.A Marketing logo used by the web app.
- `assets/icon.png` and `assets/splash.png` — source artwork for Android icon/splash generation.
- `capacitor.config.json` — Android app name and package ID.
- `.github/workflows/build-apk.yml` — builds the APK on GitHub Actions.

## Build APK on GitHub (no Android Studio required)

1. Create a new **Public** or **Private** repository on GitHub named `aa-marketing-apk`.
2. Upload the **contents of this folder** to the repository's root. Do not upload the ZIP file itself.
3. Open the repository's **Actions** tab.
4. Select **Build A.A Marketing APK** and press **Run workflow**. (A push to `main` or `master` also starts a build.)
5. Wait for the workflow to finish successfully.
6. Open the completed workflow run, scroll to **Artifacts**, and download **A-A-Marketing-APK**.
7. Extract the downloaded artifact ZIP. The APK inside is `app-debug.apk`.

## App identity

- Display name: `A.A Marketing`
- Android application ID: `com.aamarketing.app`

## Important

- This workflow creates a **debug APK** suitable for testing and direct installation. Android may show a warning when installing an APK downloaded outside the Play Store.
- A signed release APK / Play Store package requires a private signing key and credentials. Do not publish signing passwords in this repository.
- The project content and property information are carried over from the supplied source. Verify all rates, claims, maps, contact details and project status before public release.
