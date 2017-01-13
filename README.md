## Cordova - Androïd with OSX
Source : https://cordova.apache.org/docs/fr/latest/guide/platforms/android/index.html

### Prerequisites :

* Install : `oh-my-zsh latest`
* Install : `Node.js 4.2.6`
* Install : `npm 2.14.12`
* Install : `ngnix`

### How install the environement Cordova with Androïd Studio ?

#### JDK 8 :

* Go to : `http://www.oracle.com/technetwork/java/javase/downloads/jdk7-downloads-1880260.html`
* Version of file : `Mac OS X	227.39 MB  	jdk-8u111-macosx-x64.dmg`
* Install the `jdk-8u111-macosx-x64.dmg`

#### Android Studio :

* Go to : `https://developer.android.com/studio/install.html`
* Download the last version `Android Stuido` and install.
* Modify your `.bashrc` or `.zshrc` and add that line : `export PATH=${PATH}:/Development/android-sdk/platform-tools:/Development/android-sdk/tools`.
* Open Androïd Sutio and repsect the next steps of configuration.
* Open the SDK manager and install thes version of `SDK 5.1.1` with `l'API 22`, with `SDK build-tool 19.1.0`.
* Configuring a AVD whit the `version 5.1.1` create the project with a image system by default.
* Run directly the emulator with the versiob `5.1.1` Androïd with the applicaton by default.

### Cordova :

We will now create the web application with Node.js and Cordova.

#### Create the package npm :

* Install the last version of `Node@4.2.6` and `npm@2.14.12`.
* Create a repository wtih the name `app-mobile-android`.
* Enter in the repository and execute the CLI : `npm init` on your terminal and follow step by step.

#### Create a project with Cordova :

* Install `Cordova` in global of your computer with CLI : `npm i cordova -g`.
* Create app Cordova CLI : `cordova create lib com.app.lib appFonderie`.
* Add for the next step a project with Androïd : `cordova platform add android` the project will fit automaticaly and dowload all dependences.
* Open the repositroy root with a editor Ouvrez le repertoire racine avec un IDE, you should have in ./www with ./css ./img et ./js.
* After of run your application you should build your application with Cordova. CLI : `cordova build android` the `.apk` is generated.
* For run the emulator by default use the CLI : `cordova emulate android`.
* For run the emulator with our emulator launch CLI : `cordova emulate android`.
* For run the application with my device connected run CLI : `cordova run android --device`.