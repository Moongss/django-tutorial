## Django 설치하기

이제 가상 환경을 사용하는 법을 알고 있으니 가상 환경에 Django(이하 장고)를 설치하는 절차를
밟아보도록 해요.

### pip 업그레이드

장고를 설치하기 전에, 장고 설치에 필요한 `pip`가 최신 버전이 아닐 수도 있으니 다음의
명령어를 입력해서 업그레이드해봅시다! (이미 최신 버전이라면 이미 최신 버전이라고 출력될
거예요.)

``` bash
(<venv>) [<root>]$ python -m pip install --upgrade pip
```

### requirements 를 이용해 패키지 설치하기

requirements 파일은 `pip install` 을 이용해 설치할 의존성들의 목록을 보관합니다.

코드 편집기를 이용해 `djangogirls/` 폴더 안에 `requirements.txt` 파일을 생성해 주세요:

``` txt
djangogirls
└───requirements.txt
```

`djangogirls/requirements.txt` 파일 내에 다음과 같은 내용을 추가해 주세요.

``` txt
Django~=2.0.6
```

이제 준비는 끝났으니 장고를 설치해 봐요. `pip install -r requirements.txt` 를 실행해 주세요.

``` bash
(myvenv) ~$ pip install -r requirements.txt
Collecting Django~=2.0.6 (from -r requirements.txt (line 1))
  Downloading Django-2.0.6-py3-none-any.whl (7.1MB)
Installing collected packages: Django
Successfully installed Django-2.0.6
```

#### 장고 설치: Windows

윈도우에서 pip 를 호출했을때 에러가 발생한다면, 여러분의 프로젝트 경로가 공백이나 특수문자를
포함했는지 (ex: `C:\Users\User Name\djangogirls`) 확인해 보세요. 만약 포함되어 있다면
공백이나 특수문자가 없는 경로 (`C:\djangogirls` 정도면 적당할 것 같네요) 를 이용해 주시기
바랍니다. 새 디렉토리에 가상환경을 새로 준비하고 기존의 것을 삭제한 뒤, 앞의 명령어를 다시
시도해주세요. (가상 환경은 절대경로를 이용하기 때문에 가상 환경 디렉토리는 이동하시면
안돼요!)

#### 장고 설치: Windows 8, Windows 10

만약 장고를 설치하려 할때 명령 창(command line) 이 멈추는 현상이 일어난다면,
앞의 명령어 대신 다음 명령어을 이용해 주세요.

```bash
C:\Users\Name\djangogirls> python -m pip install -r requirements.txt
```

#### 장고 설치: Linux

Ubuntu 12.04 버전에서 pip 를 호출할 때 에러가 발생한다면,
`python -m pip install -U --force-reinstall pip` 를 이용해 가상환경 내의 pip 를
재설치 해주세요.

드디어 끝났네요! 이제 장고 어플리케이션을 만들어 봐요!
