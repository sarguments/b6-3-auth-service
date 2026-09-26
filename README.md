# B6-3 로그인이 되고 회원끼리 연결되는 웹 서비스 만들기

코딧세이 AI 올인원 본과정 B6-3 미션 저장소입니다.

## 소재
스마트팩토리·로봇을 소재로 삼는다. 정비 담당자 계정과 권한을 다루는 서비스를 만든다. 로그인과 담당자 사이의 연결을 다룬다.
미션 요구사항과 제약은 원문을 그대로 따르고, 소재는 데이터·예시·문구 범위에서만 바꾼다.

## 범위
B6-2 확장·Depends 인증/인가·모델 3개+ 연관관계·상태 변경 비즈니스 로직

## 개발 환경
Python 3.10 이상과 FastAPI 기반 환경을 사용합니다. 핵심 패키지 fastapi, uvicorn, sqlalchemy, jinja2, python-multipart는 requirements.txt에 기록했습니다.
인증 관련 패키지는 선택한 방식에 맞춰 python-jose, passlib, bcrypt, itsdangerous, starlette의 허용 범위에서 결정합니다.

### 새 환경에서 준비

Git을 설치한 뒤 새 기기에서 저장소를 받습니다.

```bash
git clone https://github.com/sarguments/b6-3-auth-service.git
cd b6-3-auth-service
```

Python 3.10 이상을 설치한 뒤 저장소 루트에서 실행합니다. 가상환경은 기기마다 새로 만듭니다.

```bash
python3 --version
python3 -m venv .venv
.venv/bin/python --version
.venv/bin/python -m pip install -r requirements.txt
```

현재 의존성 파일에는 공통 핵심 패키지 이름만 있습니다. 인증 방식에 필요한 선택 패키지와 서버 실행 명령은 구현·검증 후 기록합니다.

## 준비 상태
Python 3.14.3 가상환경을 준비했습니다. 외부 의존성은 아직 설치하지 않았습니다. 인증·인가·모델 관계와 상태 변경 로직은 B6-2 이후 직접 구현합니다.
