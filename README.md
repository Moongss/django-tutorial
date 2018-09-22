# Django 튜토리얼

Django 튜토리얼 책의 소스 레포지토리입니다.
책을 읽고 싶으시다면 [이곳](https://oslint.github.io/books/django-tutorial)으로 가주세요.

## 빌드

### 요구 사항

이 책을 빌드하는 데에는 최소 v0.0.13 버전 이상의 [mdBook](https://github.com/rust-lang-nursery/mdBook)이 필요합니다. (v0.2.0 이상을 권장합니다.)

mdBook을 설치하는 방법은 [mdBook 레포지토리의 README.md의 Installation 문단](https://github.com/rust-lang-nursery/mdBook/blob/master/README.md#installation)에 나와 있습니다.

### 빌드하는 법

이 책을 빌드하려면 우선 `cd`를 이용해 이 프로젝트의 최상위 디렉토리로 이동합니다. 그 후 다음의 명령어를 입력하세요.

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

## 번역

### 작업 방식

<https://tutorial.djangogirls.org/en/> 를 기준으로 하며, 내용 구조의 변화를 주었습니다.

새 구조는 `src` 폴더 내의 `SUMMARY_future` 에 작성되어 있으며,
이 구조를 참고하여 작업하시면 됩니다.

문서 구조 (chapter, section) 는 다음과 같이 번역해 주시기 바랍니다.

- chapter: 장, 챕터
- section: 절, 구간

마지막으로, 다른 작업자들을 배려해 가급적 한 줄의 길이가 100 을 넘어가지 않도록
적절히 줄바꿈을 해 주시길 바랍니다. (Markdown의 문법이 깨질 경우는 예외)

### 번역 용어

번역하기 애매할 경우 무리하게 번역하지 않고 원어를 그대로 사용하며,
아래 정리되어 있는 용어 또한 문체에 맞게 변형해야 할 경우
의미에 혼동이 없는 범위 내에서 어느정도의 변형이 가능합니다.

만약 기존에 없던 새로운 단어가 나타날 경우, 처음 나타날 때 괄호를 이용해
원어를 적어주시기 바랍니다. (가상 환경(virtualenv) 은 ~)

#### 번역 용어 정리 (abc 순)

여러개가 있는 경우 가급적 앞 순서의 용어를 이용합니다.

- command line: 명령 창
- directory: 디렉토리
- django: 장고
- python: 파이썬
- virtualvenv: 가상 환경

## 라이선스

Django 튜토리얼은 [Creative Commons Attribution-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-sa/4.0/)에 준수하여 [Django Girls Tutorial](https://github.com/DjangoGirls/tutorial)을 기초로 하여 작성되었습니다.
