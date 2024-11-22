This is an updated version of the Demo app for the "Build Offline-Enabled Mobile Apps With Ionic and Couchbase Lite" talk at Couchbase Connect 2021. The app allows users to search and bookmark hotels using data loaded from a Couchbase Lite database.

This app is build on Capacitor 6 - and it's recommended you have a basic understanding of Capacitor and Ionic before running this app.

[Capacitor docs](https://capacitorjs.com/docs/basics/workflow)
[Ionic docs](https://ionicframework.com/docs/core-concepts/cross-platform)


## Features

* Data from a Couchbase Lite database: The database is embedded into the Android and iOS apps.

* Plugin is designed using Capacitor 

* UI components powered by Ionic Framework: search bar, bookmarks, icons, list items, and more.

* Bookmarked hotels: Saved in a Couchbase Lite database.

* Cross-platform: Create iOS and Android apps from the same codebase.

## Tech Details

- UI: [Ionic Framework 8](https://ionicframework.com) and [Angular 17](https://angular.io)
- Native runtime: [Capacitor 6](https://capacitorjs.com)
- Database: Couchbase Lite v3.2.1 using [CBL-Ionic](https://cbl-ionic.dev)

## How to Run

Note: Installing and running this app, which uses Couchbase Lite Enterprise Edition, requires a license from Couchbase.

- Install the Ionic CLI: `npm install -g @ionic/cli`

- Clone the repo:
```shell
git clone git@github.com:couchbaselabs/cbl-ionic-hotels-angular.git
```

- Install the dependencies for the demo app 
    ```shell
    cd cbl-ionic-hotels-angular
    npm install
    cd ios/App
    pod install
    cd ../..
    ```

- Build the app:
```shell 
  npm run build
  npx cap sync
 ```
 - Run via capacitor (recommended)
 **iOS**
 ```shell
   ionic capacitor run ios -l --external 
 ```
 **Android**
 ```shell
   ionic capacitor run android -l --external
 ```
 
