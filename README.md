# Character Reference Studio

This version is intentionally **project-agnostic**.

## Architecture

- Projects are independent libraries.
- Characters belong to projects.
- References can represent characters, outfits, locations, props, creatures, styles, poses, etc.
- Image-generation providers are global and independent of projects.
- Projects can be exported/imported as JSON backups.
- The app does not hard-code Kareem, Elena, or any other project.

## Desktop

Install Node.js, then:

```bash
npm install
npm run start
```

To build Windows installers:

```bash
npm run desktop
```

The `dist/` folder will contain the generated Windows installer/portable build.

## Android

Install Android Studio and the Android SDK. Then:

```bash
npm install
npx cap add android
npm run android
npm run android:open
```

Build an APK from Android Studio.

## Important

The generation workspace is provider-neutral. The UI stores provider endpoint information, but a production app should use a secure backend/proxy rather than exposing permanent API keys inside a client app.

The current project is a management/library shell; the next adapter layer can connect different image-generation APIs without changing the project/library structure.
