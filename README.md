# 폴더생성 및 이동
cd ~ 
mkdir Django_first
cd Django_first

# 폴더에서 재 시작
code -r .

# 가상환경 생성
uv venv .venv

# 가상환경 실행
source .venv/bin/activate      # macOS / Linux

# uv pip 최신화
uv pip install --upgrade pip

# 가상환경 초기화
uv init

# django 추가 , 주의사항 : 가상환경이 켜진 상태 확인
uv add django
uv pip freeze > requirements.txt
# 버전 배포용 명령어    ( 현재 생략 )
uv pip install -r requirements.txt

# 설치확인
python -m django --version
> 6.0.1  