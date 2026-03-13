# mini_project_0313
Traffic Monitoring and Anomaly Detection


Frontend====================================================================================

cmd에서

# 프론트엔드 폴더로 이동
cd frontend_js

npm install

npm run dev


Backend=====================================================================================

backend_flask 안의 migrations 폴더 지우기

cmd에서

# 백엔드 폴더로 이동
cd backend_flask

# 새로운 가상환경 만들기
conda create -n tads python=3.11 -y
conda activate tads

pip install -r requirements.txt

=======================.env==========================
아래 내용을 넣어서 .env로 저장하고 프로젝트 폴더에 추가

# Flask Settings
FLASK_APP=app.py
FLASK_ENV=development
SECRET_KEY=your_generated_random_secret_key

# Database Settings
DB_USER=root
DB_PASSWORD=12341234
DB_HOST=localhost
DB_PORT=3306
DB_NAME=tads

# Application Settings
PORT=5000
HOST=0.0.0.0

# ITS API Settings
ITS_API_KEY=22f088a782aa49f6a441b24c2b36d4ec

# Flask Settings
FLASK_APP=app.py
FLASK_ENV=development
SECRET_KEY=your_generated_random_secret_key

# Database Settings
DB_USER=root
DB_PASSWORD=12341234
DB_HOST=localhost
DB_PORT=3306
DB_NAME=tads

# Application Settings
PORT=5000
HOST=0.0.0.0

# ITS API Settings
ITS_API_KEY=22f088a782aa49f6a441b24c2b36d4ec

# Kakao Map API Settings
VITE_KAKAO_MAP_API_KEY=de202e5f1e1b8c26cb092fb674de768d

# Detection Settings
CONFIDENCE_THRESHOLD=0.66

# Detection Settings
CONFIDENCE_THRESHOLD=0.66
====================================================

# DB 초기화
workbench나 vscode database에서
CREATE DATABASE tads;

cmd에서 

flask db init

flask db migrate -m "message"

flask db upgrade

python app.py로 실행

Simulation===================================================================================

N드라이브/이동훈/assets 폴더 다운 받아서
backend_flask/ 에 넣으면 정상동작.
