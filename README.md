
# NativeScript Installation for mac

> 네이티브 스크립트 설치 방법 MAC

## 1. Install Node.js (최신버전 Node 설치)

``` bash
# The NativeScript CLI is built on Node.js, and as such you need to have Node.js installed to use NativeScript
install the latest “LTS” (long-term support)
```
<https://nodejs.org/>

## 2. Install the NativeScript CLI (NativeScript CLI 설치)
``` bash
# sudo npm install -g nativescript (If you’re on macOS and receive an EACCES error)
npm install -g nativescript
```

## 3. Install iOS and Android requirements (IOS/Android 설치)
``` bash
ruby -e "$(curl -fsSL https://www.nativescript.org/setup/mac)"
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

## 7. Install JDK 8 (JDK 8 설치 및 세팅)
Install JDK 8
``` bash
vi ~/.bash_profile or vi ~/.zshrc
export JAVA_HOME=$(/usr/libexec/java_home)
```

## 8. cocoapods (cocoapods 설치)
``` bash
sudo gem install cocoapods
```




## 9. Verify the setup (이상유무 확인)
``` bash
tns doctor
```

