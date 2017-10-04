# test

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 1.4.4. Install angular-cli globally, using npm i @angular-cli -g

## Development server

Run `npm start` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `npm run build` to build the project. The build artifacts will be stored in the `www/` directory. 

## Running unit tests

Run `npm run test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `npm run e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).

For mobile building (general setup):
1. Install cordova, using: `npm i cordova -g`
2. Use cordova prepare for restore all necessary platforms.
3. For run app use `cordova run ios|android|browser`. Use `--device`, for running on device. (Application should have signification and device should be connected to Your Mac)
3. For release build app use `sudo npm run release-ios|release-android`. (Application should have signification)

For Android run\build you should have:
1. [Java Development Kit](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html). Minimum 7 version
2. Set `JAVA_HOME` environment variable, using `export JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk1.8.0_144.jdk/Contents/Home`
3. Install [Android Studio] or [SDK Android Stand-alone SDK Tools](https://developer.android.com/studio/index.html).
4. Add emulator to system.
5. Update `PATH` variable, using `export PATH=${PATH}:/Development/android-sdk/platform-tools:/Development/android-sdk/tools`.
6. Update ANDROID_HOME variable, using `export ANDROID_HOME=~/Library/Android/sdk/`
7. Before running `release-android` remove test.apk from root folder.
8. For standalone build use `sudo npm run release-android` and `npm run build-android` for debug. Password for `android-release.jks` is `q1w2e3r4`. (test.apk will be at the root of Your application as test.apk)

For ios run\build you should have: 
1. XCode and connected certificate. You should be in Your development team () to have an ability for building. You should have this [settings](http://prntscr.com/gspymx) (Team ID can be another. If it will be another, change it, if You want to build);
2. Open <YOUR_PROVISION_PROFILE>.mobileprovision. It will save Your file in `~/Libary/MobileDevices/Provisioning\ Profile/` with uniq id. 
Open this folder, choose last file, copy ID and pass to the console, using `export PROVISIONING_PROFILE_NAME=XXXX-XXXX-XXXX-XXXX` (for example, asdasd-asdas-asdasd-921a2-123asd).
3. Run `sudo npm run release-ios` for standalone application and `sudo npm run build-ios` for debug. (test.ipa will be at `<YOUR_PATH_TO_PROJECT>/platforms/ios/build/device/`)

Full building:
1. For full building, You should have all environment variables, like PATH, ANDROID_HOME, JAVA_HOME, etc.
2. Run `sudo npm run full-release-build`

