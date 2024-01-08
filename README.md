# fullstack-gpt

# 1. virtual environment

## 가상환경 생성

- `python -m venv ./env` 파이썬 3.3 버전 이후부터는 새로운 가상환경을 생성할 수 있다. 현재 디렉터리에 새로운 가상환경 만들기.
- `git init .` 깃 레포지토리 설정해주기. `echo env/ > .gitignore` 깃이그노어 파일 생성하면서 env/ 넣어서 트래킹 제외해주기.

## 가상환경 실행

- 사용하는 os 플랫폼마다 실행하는 방법이 다르다. 사용하는 터미널에 따라서 명령어가 다르다. <venv>는 가상환경 디렉터리를 의미한다. 현재 가상환경 이름은 env. 더 자세한 내용은 다큐멘터리 참고하기. [파이썬 가상환경 다큐멘터리](https://docs.python.org/ko/3/library/venv.html)
    - windows cmd.exe `C:\> <venv>\Scripts\activate.bat`  bash/zsh `$ source <venv>/bin/activate`
- requrements.txt 파일 생성하고 아래 링크의 디펜던시를 복사해주자. gpt apps에 필요한 기본적인 디펜던시 모음. [gpt app dependency](https://gist.github.com/serranoarevalo/72d77c36dde1cc3ffec34105eb666140)
    - `pip install -r requirements.txt` 디팬던시 설치하기

## api 키 관리

- `echo OPENAI_API_KEY="" > .env` .env 파일 생성하면 openai 관리키 써주기. 따옴표 안에 openai 키값을 써주자.
- 깃이그노어 파일에 `.env` 추가해서 트래킹 제외하기.