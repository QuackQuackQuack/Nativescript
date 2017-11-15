
# NativeScript Installation for mac

> 네이티브 스크립트 설치 방법 MAC

## 간단설치
### 1. Install Node.js (최신버전 Node 설치)

``` bash
# The NativeScript CLI is built on Node.js, and as such you need to have Node.js installed to use NativeScript
install the latest “LTS” (long-term support)
```
<https://nodejs.org/>

### 2. Install the NativeScript CLI (NativeScript CLI 설치)
``` bash
# sudo npm install -g nativescript (If you’re on macOS and receive an EACCES error)
npm install -g nativescript
```

## 3. Install iOS and Android requirements (IOS/Android 설치)
``` bash
(sudo) ruby -e "$(curl -fsSL https://www.nativescript.org/setup/mac)"
```

## 4. HomeBrew  (홈브류 설치)
``` bash
# Install Homebrew to simplify the installation process. (홈브류 없을 경우)
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

# 홈브류 있는경우
brew update
brew install node@6
```

## 5. Xcode (Xcode 설치 IOS)
```bash
xcode 최신 버전 설치 or Update

sudo gem install xcodeproj
```
<https://developer.apple.com/download/more/>

## 6. cocoapods (cocoapods 설치)
``` bash
sudo gem install cocoapods
```

## 7. Install JDK 8 (JDK 8 설치 및 세팅)
Install JDK 8
<http://download.oracle.com/otn-pub/java/jdk/8u151-b12/e758a0de34e24606bca991d704f6dcbf/jdk-8u151-macosx-x64.dmg>

Set the JAVA_HOME system environment variable (환경변수 설정)
``` bash
vi ~/.bash_profile or vi ~/.zshrc
export JAVA_HOME=$(/usr/libexec/java_home)

#8버전 사용
export JAVA_HOME=$(/usr/libexec/java_home -v 1.8)
```
Install the Android SDK. (안드로이드 스튜디오 설치)
안드로이드 스튜디오 설치시 custom > AVD 같이 설치
<https://developer.android.com/studio/index.html>
AVD 세팅
<https://docs.nativescript.org/tooling/android-virtual-devices>
<https://developer.android.com/studio/run/managing-avds.html?hl=ko>

brew cask install android-sdk
(안드로이드 스튜디오 설치 후에도 설치가 되지 않았다고 나올시)
``` bash
brew cask install android-sdk
```

Set the ANDROID_HOME system environment variable (환경변수 설정)
``` bash
# NativeScript Guide
export ANDROID_HOME=/usr/local/share/android-sdk

# run error 로 인한 변경
export ANDROID_HOME=/Users/{userName}/Library/Android/sdk
export ANDROID_SDK_ROOT=$ANDROID_HOME
```

Android SDK Platform 25, Android SDK Build-Tools 25.0.2 or later, Android Support Repository
``` bash
$ANDROID_HOME/tools/bin/sdkmanager "tools" "platform-tools" "platforms;android-25" "build-tools;25.0.2" "extras;android;m2repository" "extras;google;m2repository"
```

## 9. Verify the setup (이상유무 확인)
``` bash
tns doctor
```

