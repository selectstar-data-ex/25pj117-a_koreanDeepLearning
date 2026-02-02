# 25pj117-a_koreanDeepLearning
- 25pj117-a_한국딥러닝 : 데이터 오류 체크 코드

## 코드 목적
- 25pj117-a_한국딥러닝 손글씨 인식을 위한 코드

## 작성자
- 최서현

## 폴더 내용
- `data/`: 원본 데이터셋 및 전처리된 데이터 보관
- `src/`: 핵심 로직 소스 코드
  - `preprocess.py`: 데이터 노이즈 제거 및 라벨링 오류 체크 스크립트
  - `model.py`: 딥러닝 모델(CNN/Transformer 등) 정의
  - `train.py`: 모델 학습 실행 파일
- `checkpoints/`: 학습된 모델 가중치(.pth, .h5) 저장 폴더
- `utils/`: 시각화 및 로그 기록을 위한 보조 도구
- `requirements.txt`: 프로젝트 실행을 위한 라이브러리 목록

## 사용방법

### 1. 환경 설정
먼저 필요한 라이브러리를 설치합니다.
```pip install -r requirements.txt```

### 2. 2. 데이터 오류 체크
학습 전 데이터셋의 결측치나 라벨링 오류를 검사합니다.
```python src/preprocess.py --data_path ./data/raw --check_error True```
~~
