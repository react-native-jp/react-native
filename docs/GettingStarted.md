---
id: quick-start-getting-started
title: はじめに
layout: docs
category: The Basics
permalink: docs/getting-started.html
next: tutorial
---

React Nativeへようこそ！  
React Nativeを導入するためのページです。すぐにアプリケーションを構築できます。  
React Nativeが既にインストールされている場合は、
[チュートリアル](docs/tutorial.html)に進んでください。

導入方法は、開発オペレーティングシステムによって異なります。  
また、iOSまたはAndroid向けに開発を開始するかどうかでも異なります。  
iOSとAndroidの両方で開発したいのであれば、それは問題ありません。  
しかし設定が少し異なるので、最初から選択する必要があります。

<div class="toggler">
  <style>
    .toggler a {
      display: inline-block;
      padding: 10px 5px;
      margin: 2px;
      border: 1px solid #05A5D1;
      border-radius: 3px;
      text-decoration: none !important;
    }
    .display-os-mac .toggler .button-mac,
    .display-os-linux .toggler .button-linux,
    .display-os-windows .toggler .button-windows,
    .display-platform-ios .toggler .button-ios,
    .display-platform-android .toggler .button-android {
      background-color: #05A5D1;
      color: white;
    }
    block { display: none; }
    .display-platform-ios.display-os-mac .ios.mac,
    .display-platform-ios.display-os-linux .ios.linux,
    .display-platform-ios.display-os-windows .ios.windows,
    .display-platform-android.display-os-mac .android.mac,
    .display-platform-android.display-os-linux .android.linux,
    .display-platform-android.display-os-windows .android.windows {
      display: block;
    }
  </style>
  <span>モバイルOS:</span>
  <a href="javascript:void(0);" class="button-ios" onclick="display('platform', 'ios')">iOS</a>
  <a href="javascript:void(0);" class="button-android" onclick="display('platform', 'android')">Android</a>
  <span>開発OS:</span>
  <a href="javascript:void(0);" class="button-mac" onclick="display('os', 'mac')">macOS</a>
  <a href="javascript:void(0);" class="button-linux" onclick="display('os', 'linux')">Linux</a>
  <a href="javascript:void(0);" class="button-windows" onclick="display('os', 'windows')">Windows</a>
</div>

<block class="linux windows ios" />

## サポートされていません

<div>残念ながら、MacでしかiOS用に開発することはできません。iOSアプリを構築したいがまだMacをお持ちでない場合は、<a href="" onclick="display('platform', 'android')">Android</a>の手順から始めてみてください。</div>

<center><img src="img/react-native-sorry-not-supported.png" width="150"></img></center>

<block class="mac ios" />

## 依存関係のインストール

開発にはNode.js, Watchman, React Nativeコマンドラインインターフェース, Xcodeが必要です。

<block class="mac android" />

## 依存関係のインストール

開発にはNode.js, Watchman, React Nativeコマンドラインインターフェース, Android Studioが必要です。

<block class="windows linux android" />

## 依存関係のインストール

開発にはNode.js, Watchman, React Nativeコマンドラインインターフェース, Android Studioが必要です。

<block class="mac ios android" />

### Node, Watchman

[Homebrew](http://brew.sh/)を使用してNodeおよびWatchmanをインストールすることをお勧めします。  
Homebrewをインストールした後、ターミナルで次のコマンドを実行します:

```
brew install node
brew install watchman
```

> [Watchman](https://facebook.github.io/watchman)はファイルシステムの変更を監視するためのFacebookのツールです。  
より良いパフォーマンスを得るためにインストールすることを強くお勧めします。

<block class="linux android" />

### Node

[Linuxディストリビューションのインストール手順](https://nodejs.org/en/download/package-manager/)に従って、Node.js 4以降をインストールしてください。

<block class='windows android' />

### Node

Node.jsとPython2は、Windows用の一般的なパッケージマネージャである[Chocolatey](https://chocolatey.org)を利用してインストールすることをお勧めします。  
管理者としてコマンドプロンプトを開き、次のコマンドを実行します:

```
choco install nodejs.install
choco install python2
```

> 追加のインストールオプションは、[Node.jsのダウンロードページ](https://nodejs.org/en/download/)で見つけることができます。

<block class="mac ios android" />

### React Nativeコマンドラインインターフェース

Node.jsにはnpmが付属しており、React Nativeコマンドラインインターフェイスをインストールできます。

ターミナルで次のコマンドを実行します:

```
npm install -g react-native-cli
```

> If you get an error like `Cannot find module 'npmlog'`, try installing npm directly: `curl -0 -L https://npmjs.org/install.sh | sudo sh`.

<block class="windows linux android" />

### The React Native CLI

Node.js comes with npm, which lets you install the React Native command line interface.

Run the following command in a Terminal:

```
npm install -g react-native-cli
```

> 次のようなエラーが発生した場合、Cannot find module 'npmlog', npmを直接インストールしてください: curl -0 -L http://npmjs.org/install.sh | sudo sh.

<block class="mac ios" />

### Xcode

Xcodeをインストールする最も簡単な方法は、[Mac App Store](https://itunes.apple.com/us/app/xcode/id497799835?mt=12)経由です。  
Xcodeをインストールすると、iOSシミュレータとiOSアプリを構築するのに必要なすべてのツールもインストールされます。

<block class="mac linux windows android" />

### Android開発環境

Android開発が初めての方にとって、開発環境の設定は面倒です。  
既にAndroid開発に精通している場合も、設定が必要な場合があります。  
いずれの場合も、次のステップに注意深く従ってください。

#### 1. Android Studioをダウンロードしてインストールしてください

[Android Studio](https://developer.android.com/studio/install.html)には、React Nativeアプリの実行とテストに必要なAndroid SDKとAVD(エミュレータ)が用意されています。

<block class="mac android" />

> Android Studioには、[Java SE Development Kit(JDK)](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)バージョン8が必要です。ターミナルにjavac -versionを入力して、使用しているバージョンがある場合は確認できます。

```
$ javac -version
javac 1.8.0_111
```

> バージョン`1.8.x_xxx`はJDK 8に対応しています。

<block class="mac windows android" />

#### 2. Install the AVD and HAXM

Choose `Custom` installation when running Android Studio for the first time. Make sure the boxes next to all of the following are checked:

- `Android SDK`
- `Android SDK Platform`
- `Performance (Intel ® HAXM)`
- `Android Virtual Device`

Then, click "Next" to install all of these components.

> If you've already installed Android Studio before, you can still [install HAXM](https://software.intel.com/en-us/android/articles/installation-instructions-for-intel-hardware-accelerated-execution-manager-windows) without performing a custom installation.

<block class="linux android" />

#### 2. Install the AVD and configure VM acceleration

Choose `Custom` installation when running Android Studio for the first time. Make sure the boxes next to all of the following are checked:

- `Android SDK`
- `Android SDK Platform`
- `Android Virtual Device`

Click "Next" to install all of these components, then [configure VM acceleration](https://developer.android.com/studio/run/emulator-acceleration.html#vm-linux) on your system.

<block class="mac linux windows android" />

#### 3. Install the Android 6.0 (Marshmallow) SDK

Android Studio installs the most recent Android SDK by default. React Native, however, requires the `Android 6.0 (Marshmallow)` SDK. To install it, launch the SDK Manager, click on "Configure" > "SDK Manager" in the "Welcome to Android Studio" screen.

> The SDK Manager can also be found within the Android Studio "Preferences" menu, under **Appearance & Behavior** → **System Settings** → **Android SDK**.

Select the "SDK Platforms" tab from within the SDK Manager, then check the box next to "Show Package Details" in the bottom right corner. Look for and expand the `Android 6.0 (Marshmallow)` entry, then make sure the following items are all checked:

- `Google APIs`
- `Android SDK Platform 23`
- `Intel x86 Atom System Image`
- `Intel x86 Atom_64 System Image`
- `Google APIs Intel x86 Atom_64 System Image`

Next, select the "SDK Tools" tab and check the box next to "Show Package Details" here as well. Look for and expand the "Android SDK Build Tools" entry, then make sure that `Android SDK Build-Tools 23.0.1` is selected.

Finally, click "Apply" to download and install the Android SDK and related build tools.

<block class="mac windows linux android" />

#### 4. Set up the ANDROID_HOME environment variable

The React Native command line interface requires the `ANDROID_HOME` environment variable to be set up.

<block class="mac android" />

Add the following lines to your `~/.bashrc` (or equivalent) config file:

```
export ANDROID_HOME=${HOME}/Library/Android/sdk
export PATH=${PATH}:${ANDROID_HOME}/tools
export PATH=${PATH}:${ANDROID_HOME}/platform-tools
```

> Please make sure you export the correct path for `ANDROID_HOME`. If you installed the Android SDK using Homebrew, it would be located at `/usr/local/opt/android-sdk`.

<block class="linux android" />

Add the following lines to your `~/.bashrc` (or equivalent) config file:

```
export ANDROID_HOME=${HOME}/Android/Sdk
export PATH=${PATH}:${ANDROID_HOME}/tools
export PATH=${PATH}:${ANDROID_HOME}/platform-tools
```

> Please make sure you export the correct path for `ANDROID_HOME` if you did not install the Android SDK using Android Studio.

<block class="windows android" />

Go to **Control Panel** → **System and Security** → **System** → **Change settings** →
**Advanced System Settings** → **Environment variables** → **New**, then enter the path to your Android SDK.

![env variable](img/react-native-android-sdk-environment-variable-windows.png)

Restart the Command Prompt to apply the new environment variable.

> Please make sure you export the correct path for `ANDROID_HOME` if you did not install the Android SDK using Android Studio.

<block class="linux android" />

### Watchman (optional)

Follow the [Watchman installation guide](https://facebook.github.io/watchman/docs/install.html#build-install) to compile and install Watchman from source.

> [Watchman](https://facebook.github.io/watchman/docs/install.html) is a tool by Facebook for watching
changes in the filesystem. It is highly recommended you install it for better performance, but it's alright to skip this if you find the process to be tedious.

<block class="mac windows linux android" />

## Starting the Android Virtual Device

![Android Studio AVD Manager](img/react-native-tools-avd.png)

You can see the list of available AVDs by opening the "AVD Manager" from within Android Studio. You can also run the following command in a terminal:

```
android avd
```

Once in the "AVD Manager", select your AVD and click "Start...".

> Android Studio should have set up an Android Virtual Device for you during installation, but it is very common to run into an issue where Android Studio fails to install the AVD. You may follow the [Android Studio User Guide](https://developer.android.com/studio/run/managing-avds.html) to create a new AVD manually if needed.

<block class="mac ios android" />

## Testing your React Native Installation

<block class="mac ios" />

Use the React Native command line interface to generate a new React Native project called "AwesomeProject", then run `react-native run-ios` inside the newly created folder.

```
react-native init AwesomeProject
cd AwesomeProject
react-native run-ios
```

You should see your new app running in the iOS Simulator shortly.

`react-native run-ios` is just one way to run your app. You can also run it directly from within Xcode or [Nuclide](https://nuclide.io/).

<block class="mac android" />

Use the React Native command line interface to generate a new React Native project called "AwesomeProject", then run `react-native run-android` inside the newly created folder:

```
react-native init AwesomeProject
cd AwesomeProject
react-native run-android
```

If everything is set up correctly, you should see your new app running in your AVD shortly.

`react-native run-android` is just one way to run your app - you can also run it directly from within Android Studio or [Nuclide](https://nuclide.io/).

<block class="mac ios android" />

### Modifying your app

Now that you have successfully run the app, let's modify it.

<block class="mac ios" />

- Open `index.ios.js` in your text editor of choice and edit some lines.
- Hit `Command⌘ + R` in your iOS Simulator to reload the app and see your change!

<block class="mac android" />

- Open `index.android.js` in your text editor of choice and edit some lines.
- Press the `R` key twice or select `Reload` from the Developer Menu to see your change!

<block class="mac ios android" />

### That's it!

Congratulations! You've successfully run and modified your first React Native app.

<center><img src="img/react-native-congratulations.png" width="150"></img></center>

<block class="windows android" />

## Testing your React Native Installation

Use the React Native command line interface to generate a new React Native project called "AwesomeProject", then run `react-native start` inside the newly created folder to start the packager.

```
react-native init AwesomeProject
cd AwesomeProject
react-native start
```

Open a new command prompt and run `react-native run-android` inside the same folder to launch the app on your AVD.

```
react-native run-android
```

<block class="linux android" />

## Testing your React Native Installation

Use the React Native command line interface to generate a new React Native project called "AwesomeProject", then run `react-native run-android` inside the newly created folder.

```
react-native init AwesomeProject
cd AwesomeProject
react-native run-android
```

<block class="windows linux android" />

If everything is set up correctly, you should see your new app running in your Android emulator shortly.

<block class="windows android" />

> If you're targeting API level 23, the app might crash on first launch with an error smilar to `Unable to add window android.view.ViewRootImpl$W@c51fa6 -- permission denied for this window type`. To fix this, you need to go to `System settings > Apps > Configure apps > Draw over other apps` and grant the permission for the app.

NOTE: Many React Native modules haven't been tested on Marshmallow and might break. Please thoroughly test the app if you target API level 23 and file a bug report if you find that something is broken.

<block class="windows linux android" />

### Modifying your app

Now that you have successfully run the app, let's modify it.

- Open `index.android.js` in your text editor of choice and edit some lines.
- Press the `R` key twice or select `Reload` from the Developer Menu to see your change!

### That's it!

Congratulations! You've successfully run and modified a React Native app.

<center><img src="img/react-native-congratulations.png" width="150"></img></center>

<block class="mac ios" />

## Now What?

- If you want to add this new React Native code to an existing application, check out the [Integration guide](docs/integration-with-existing-apps.html).

- If you can't get this to work, see the [Troubleshooting](docs/troubleshooting.html#content) page.

- If you're curious to learn more about React Native, continue on
to the [Tutorial](docs/tutorial.html).

<block class="windows linux mac android" />

## Now What?

- If you want to add this new React Native code to an existing application, check out the [Integration guide](docs/integration-with-existing-apps.html).

- If you can't get this to work, see the [Troubleshooting](docs/troubleshooting.html#content) page.

- If you're curious to learn more about React Native, continue on
to the [Tutorial](docs/tutorial.html).

<script>
// Convert <div>...<span><block /></span>...</div>
// Into <div>...<block />...</div>
var blocks = document.getElementsByTagName('block');
for (var i = 0; i < blocks.length; ++i) {
  var block = blocks[i];
  var span = blocks[i].parentNode;
  var container = span.parentNode;
  container.insertBefore(block, span);
  container.removeChild(span);
}
// Convert <div>...<block />content<block />...</div>
// Into <div>...<block>content</block><block />...</div>
blocks = document.getElementsByTagName('block');
for (var i = 0; i < blocks.length; ++i) {
  var block = blocks[i];
  while (block.nextSibling && block.nextSibling.tagName !== 'BLOCK') {
    block.appendChild(block.nextSibling);
  }
}
function display(type, value) {
  var container = document.getElementsByTagName('block')[0].parentNode;
  container.className = 'display-' + type + '-' + value + ' ' +
    container.className.replace(RegExp('display-' + type + '-[a-z]+ ?'), '');
}

// If we are coming to the page with a hash in it (i.e. from a search, for example), try to get
// us as close as possible to the correct platform and dev os using the hashtag and block walk up.
var foundHash = false;
if (window.location.hash !== '' && window.location.hash !== 'content') { // content is default
  var hashLinks = document.querySelectorAll('a.hash-link');
  for (var i = 0; i < hashLinks.length && !foundHash; ++i) {
    if (hashLinks[i].hash === window.location.hash) {
      var parent = hashLinks[i].parentElement;
      while (parent) {
        if (parent.tagName === 'BLOCK') {
          var devOS = null;
          var targetPlatform = null;
          // Could be more than one target os and dev platform, but just choose some sort of order
          // of priority here.

          // Dev OS
          if (parent.className.indexOf('mac') > -1) {
            devOS = 'mac';
          } else if (parent.className.indexOf('linux') > -1) {
            devOS = 'linux';
          } else if (parent.className.indexOf('windows') > -1) {
            devOS = 'windows';
          } else {
            break; // assume we don't have anything.
          }

          // Target Platform
          if (parent.className.indexOf('ios') > -1) {
            targetPlatform = 'ios';
          } else if (parent.className.indexOf('android') > -1) {
            targetPlatform = 'android';
          } else {
            break; // assume we don't have anything.
          }
          // We would have broken out if both targetPlatform and devOS hadn't been filled.
          display('os', devOS);
          display('platform', targetPlatform);
          foundHash = true;
          break;
        }
        parent = parent.parentElement;
      }
    }
  }
}
// Do the default if there is no matching hash
if (!foundHash) {
  var isMac = navigator.platform === 'MacIntel';
  var isWindows = navigator.platform === 'Win32';
  display('os', isMac ? 'mac' : (isWindows ? 'windows' : 'linux'));
  display('platform', isMac ? 'ios' : 'android');
}
</script>
