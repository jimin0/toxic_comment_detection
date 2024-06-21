# 욕설 탐지 모델 웹 애플리케이션 😈 : KFF(Korean Frown Filter)
이 프로젝트는 Streamlit을 사용하여 욕설 탐지 모델을 웹 애플리케이션으로 구현한 것입니다. 사용자가 입력한 댓글이 악성 댓글인지 정상 댓글인지 판별(예측)할 수 있습니다.

## 설치 및 실행 방법

### 1. 모델 파일 준비
1. 다운로드한 모델 파일 압축을 풉니다.
2. 모델 파일들이 들어 있는 디렉토리의 경로를 기억해 둡니다.

### 2. 모델 경로 수정
1. `app.py` 파일에서 모델 경로를 실제 경로로 수정합니다.

    ```python
    model_path = '/path/to/your/unzipped/model_files'  # 실제 모델 경로로 변경
    ```

### 3. 패키지 설치
1. `requirements.txt` 파일을 사용하여 필요한 패키지를 설치합니다. 터미널이나 커맨드 프롬프트에서 다음 명령어를 실행합니다:
    ```bash
    pip install -r requirements.txt
    ```

### 4. Streamlit 설치 및 테스트
1. Streamlit을 설치합니다:
    ```bash
    pip install streamlit
    ```
2. Streamlit 설치가 잘 되었는지 확인하기 위해 다음 명령어를 실행합니다:
    ```bash
    streamlit hello
    ```
3. 콘솔창에 이메일을 입력하여 내 컴퓨터를 서버로 웹 페이지를 만듭니다.

### 5. `app.py` 실행
1. 터미널이나 커맨드 프롬프트에서 프로젝트 디렉토리로 이동합니다.
2. 다음 명령어를 실행하여 Streamlit 앱을 실행합니다:
    ```bash
    streamlit run app.py
    ```

## 사용 방법
1. 웹 브라우저에서 열리는 Streamlit 앱에서 댓글을 입력합니다.
2. '예측' 버튼을 클릭하여 댓글이 정상 댓글인지 악성 댓글인지 확인합니다.


김지민_202135749_프로젝트/      
├── 김지민_202135749_dataset.zip       # 데이터셋 압축 파일.                 
├── 김지민_202135749_model.zip     # 모델 압축 파일     
├── app.py                         # Streamlit 애플리케이션 메인 파일     
├── kff.ipynb                      # Jupyter 노트북 파일   
├── kff.py                         # 파이썬 파일    
└── requirements.txt               # 필요한 Python 패키지 목록       


- `김지민_202135749_dataset.zip`: 데이터셋 파일입니다. 필요에 따라 압축을 해제하여 사용합니다.
- `김지민_202135749_model.zip`: 모델 파일입니다. 필요에 따라 압축을 해제하여 사용합니다.
- `app.py`: Streamlit 애플리케이션의 메인 파일입니다.
- `kff.ipynb`: Jupyter 노트북 파일입니다. 데이터 분석이나 모델 학습 과정이 포함되어 있을 수 있습니다.
- `kff.py`: Python 스크립트 파일입니다.
- `requirements.txt`: 필요한 Python 패키지 목록입니다.

## 요구 사항
- `python 3.x`
- `streamlit==1.36.0`
- `torch==2.3.1`
- `transformers==4.41.2`


