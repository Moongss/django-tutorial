# Django 튜토리얼

Django 튜토리얼 책의 소스 레포지토리입니다. 책을 읽고 싶으시다면 [이곳](https://oslint.github.io/books/DjangoTutorial)으로 가주세요.

## 빌드

### 요구 사항

이 책을 빌드하는 데에는 최소 v0.0.13 버전 이상의 [mdBook](https://github.com/rust-lang-nursery/mdBook)이 필요합니다. (v0.2.0 이상을 권장합니다.)

mdBook을 설치하는 방법은 [mdBook 레포지토리의 README.md의 Installation 문단](https://github.com/rust-lang-nursery/mdBook/blob/master/README.md#installation)에 나와 있습니다.

### 빌드하는 법

이 책을 빌드하려면 우선 `cd`를 이용해 DjangoTutorial의 최상위 디렉토리로 이동합니다. 그 후 다음의 명령어를 입력하세요.

```bash
mdbook build
```

빌드된 출력물은 최상위 디렉토리 아래에 새로 생성된 `book` 디렉토리에 있습니다. 확인하려면 웹 브라우저에서 열어보세요.

- *[Firefox](https://mozilla.org/firefox/new/)*

```bash
firefox book/index.html                       # Linux
open -a "Firefox" book/index.html             # macOS
Start-Process "firefox.exe" .\book\index.html # Windows(PowerShell)
start firefox.exe .\book\index.html           # Windows(cmd.exe)
```

- *[Chrome](https://www.google.com/chrome/)*

``` bash
google-chrome book/index.html                # Linux
open -a "Google Chrome" book/index.html      # macOS
Start-Process "chrome.exe" .\book\index.html # Windows(PowerShell)
start chrome.exe .\book\index.html           # Windows(cmd.exe)
```

## 라이선스

Django 튜토리얼은 [Creative Commons Attribution-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-sa/4.0/)에 준수하여 [Django Girls Tutorial](https://github.com/DjangoGirls/tutorial)을 기초로 하여 작성되었습니다.