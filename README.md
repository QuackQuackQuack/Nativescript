
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
# sudo npm install -g nativescript (If you’re on macOS and receive an EACCES erro)
npm install -g nativescript
```

## 3. Install iOS and Android requirements (IOS/Android 설치)
``` bash
ruby -e "$(curl -fsSL https://www.nativescript.org/setup/mac)"
```

## 4. Verify the setup (이상유무 확인)
``` bash
tns doctor
```
