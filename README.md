# Build Your First Ionic App: Photo Gallery (Ionic React and Capacitor)

Get started with Ionic by building a photo gallery app that runs on iOS, Android, and the web - with just one codebase. This is the complete project referenced in the ["Your First App: React" guide](https://ionicframework.com/docs/react/your-first-app). Follow along to create a complete CRUD (create-read-update-delete) experience.

Powered by [Ionic React](https://ionicframework.com/docs/react) (web app) and [Capacitor](https://capacitor.ionicframework.com) (native app runtime).

## How It Works

After the user navigates to Tab 2 (Photos), they can tap/click on the camera button to open up the device's camera. After taking or selecting a photo, it's stored permanently into the device's filesystem. When the user reopens the app at a later time, the photo images are loaded from the filesystem and displayed again in the gallery. The user can tap on a photo to be presented with the option to remove the photo.

## Feature Overview

- App framework: [React](https://reactjs.org/)
- UI components: [Ionic Framework](https://ionicframework.com/docs/components)
  - Camera button: [Floating Action Button (FAB)](https://ionicframework.com/docs/api/fab)
  - Photo Gallery display: [Grid](https://ionicframework.com/docs/api/grid)
  - Delete Photo dialog: [Action Sheet](https://ionicframework.com/docs/api/action-sheet)
- Native runtime: [Capacitor](https://capacitor.ionicframework.com)
  - Taking photos: [Camera API](https://capacitor.ionicframework.com/docs/apis/camera)
  - Writing photo to the filesystem: [Filesystem API](https://capacitor.ionicframework.com/docs/apis/filesystem)
  - Storing photo gallery metadata: [Storage API](https://capacitor.ionicframework.com/docs/apis/storage)

## Project Structure

- Tab2 (Photos) (`src/pages/Tab2.tsx`): Photo Gallery UI and basic logic.
- usePhotoGallery Hook (`src/hooks/usePhotoGallery.ts`): Logic encapsulating Capacitor APIs, including Camera, Filesystem, and Storage.

## How to Run

> Note: It's highly recommended to follow along with the [tutorial guide](https://ionicframework.com/docs/react/your-first-app), which goes into more depth, but this is the fastest way to run the app.

0. Install Ionic if needed: `npm install -g @ionic/cli`.
1. Clone this repository.
1. In a terminal, change directory into the repo: `cd photo-gallery-capacitor-react`.
1. Install all packages: `npm install`.
1. Run on the web: `ionic serve`.
1. Run on iOS or Android: See [here](https://ionicframework.com/docs/building/running).

## Features

1. Firebase hosting

### Account Info

    - App name:- react-netflix-app
    - Account:- sawannirala.09@gmail.com

### Run the following command from root folder

    - ionic build --prod
    - firebase deploy

2. Running on Web `ionic serve`

3. For android `ionic capacitor add android`, `ionic capacitor copy android` make sure you have `android-studio` installed. If you are using android>8 then add `android:usesCleartextTraffic="true"` in the `android/app/src/main/AndroidManifest.xml` like `<application android:allowBackup="true" android:icon="@mipmap/ic_launcher" android:label="@string/app_name" android:roundIcon="@mipmap/ic_launcher_round" android:supportsRtl="true" android:usesCleartextTraffic="true" android:theme="@style/AppTheme">`.

4. For Ios `ionic capacitor add ios`, `ionic capacitor open ios`

Follow this https://ionicframework.com/docs/building for more info.
