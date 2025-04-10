
# Seonmin's Github Portfolio

> 안녕하십니까!
>
> **"끊임없는 고객 중심의 사고로 신뢰와 혁신을 만들어 나갈"**
>
> **"ML 엔지니어"**
> 
> 김선민입니다!
>
> seonmin8284@gmail.com


</br>

# 📝Projects  
AI에 관한 이론적 지식과 *허깅페이스*나 *깃허브*와 같은 다양한 오픈소스들을 활용하여, 

**랭귀지, TTS, vision 등 다양한 AI 모델 파인튜닝**과 **플랫폼 서비스와 안정적인 연동 작업**을 맡아 진행했습니다.

또한, 

**과거, 프론트엔드로서 핵심 기능 구현과 플랫폼 시스템 안정화**을 맡아왔습니다.

<br />

## 1. 음성 송금 시스템(MCP_Voice_Transfer)
<details>
<summary>펼치기</summary>

- **개발기간** : 2025.04~
- **작업 범위** :  
  안드로이드 기반 음성 인터페이스 송금 시스템 설계 및 구현, FastAPI 기반 백엔드 구성,  
  음성 텍스트 → LLM 기반 의도 분석 → 시뮬레이션 송금 API 설계 및 연결,  
  Android STT+TTS 연동, 웨이크워드 기반 송금 시나리오 구현, 이상거래탐지 모델과 통합,  
  전체 시뮬레이터 및 예외 처리 설계까지 전체 End-to-End 흐름 구현

- **역할 및 업무**:
  1. **프로젝트 설계 및 백엔드 구현**
     - MCP 기반 송금 인터페이스 정의 및 FastAPI 백엔드 개발
     - 계좌 더미 생성, 시뮬레이션 송금, intent 추출 API 등 구현
     - 대화 로그 저장 및 의도 슬롯 파싱 로직 구성

  2. **음성 기반 시나리오 설계 및 인증 단계 구현**
     - `"엄마한테 3만원 보내줘"` → 웨이크워드 감지 + STT + LLM 분석 + 인증 처리 흐름 설계
     - 슬롯 누락 예외 처리 및 인증 단계 모킹 구성

  3. **성능 검증**
     - STT: WER(Word Error Rate) 측정
     - Intent/Slot: Accuracy, F1-Score 등으로 평가
     - 이상거래탐지: Precision, Recall, AUC 지표 기반 평가  
       *(IEEE-CIS Fraud Detection Dataset 활용)*

  4. **Android 연동**
     - Android STT/TTS 연동 구현
     - Retrofit 기반 FastAPI 호출 클라이언트 설계
     - VoiceInteractionService 기반 웨이크워드 감지 시스템 설계

- **기술 스택**:  
  ![Python](https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white)  
  ![FastAPI](https://img.shields.io/badge/fastapi-009688?style=for-the-badge&logo=fastapi&logoColor=white)  
  ![Flutter](https://img.shields.io/badge/flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)  
  ![Android](https://img.shields.io/badge/android-3DDC84?style=for-the-badge&logo=android&logoColor=white)

- [📎 프로젝트 상세 설명 보기](https://github.com/seonmin8284/MCP_Voice_Transfer)

</details>

<br />




## 2. 방송 스트리머를 위한 WebRTC 실시간 딥페이크 서비스
<details>
<summary>펼치기</summary>

>
> - 개발기간 : 2025.01-
> - 작업 범위 : WebRTC를 활용한 실시간 딥페이크 변환 및 스트리밍 시스템 구축, Roop 기반 Face Swap AI 모델 개발 및 최적화, Distributed Data Parallel (DDP) 기반 다중 GPU 활용 최적화, WebRTC 서버 및 TURN 서버 구축을 통한 실시간 영상 데이터 송수신 구현, Hyperstack Cloud를 활용한 서버 인프라 구축 및 RTMP 스트리밍 연계 가능성 고려  
> - 역할 및 업무:
>   
>   (1) AI 프로젝트 기획 및 설계
>   1) WebRTC 기반 실시간 딥페이크 스트리밍 서비스 기획
>   2) 주요 기능 정의 및 AI 모델(Roop + GFPGAN) 선정
>   3) WebRTC 및 AI 서버의 구조 설계 및 데이터 흐름 정의
>   
>   (2) AI 모델 개발 및 최적화
>   1) Roop 모델을 활용한 단일 이미지 Face Swap 기능 구현
>   2) InsightFace 및 GFPGAN을 활용한 얼굴 인식 및 화질 개선 적용
>   3) DDP(Distributed Data Parallel) 기반 GPU 최적화
>   
>   (3) WebRTC 스트리밍 개발
>   1) WebRTC 서버 구축 및 클라이언트 간 P2P 연결 구현
>   2) TURN 서버 구축하여 NAT/방화벽 환경에서도 안정적인 연결 보장
>   
>   (4) 서버 인프라 구축 및 배포
>   1) Hyperstack Cloud 기반으로 AI 서버, WebRTC 서버, TURN 서버 구성
>   2) Docker/Kubernetes를 활용하여 서버 컨테이너화 및 배포 자동화
>   3) RTMP 스트리밍 연계를 고려한 확장 가능성 반영
>
> - Skill : <img src="https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white"><img src="https://img.shields.io/badge/css-1572B6?style=for-the-badge&logo=css3&logoColor=white"><img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"> <img src="https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white"> 
> 
> [프로젝트 상세 설명](https://github.com/seonmin8284/realTimeDeepfake_based_on_WebRTC)

</details>

<br />

## 3. AML(Anti Money Laundering) 이상 거래 탐지를 위한 연합학습 기반 GNN(Graph neural networks) 모델 구현
<details>
<summary>펼치기</summary>

- **개발기간** : 2025.03 / 2023.01-2023.06  
- **작업 범위** :  
  개인정보 보호가 필요한 환경에서 이상거래를 탐지하기 위해,  
  GNN 기반 모델을 Federated Learning 방식으로 분산 학습시켜 구축한 시스템

- **역할 및 업무**:
  1. **모델 및 시스템 아키텍처 설계**
     - GNN 모델 (PyTorch Geometric) 기반 거래 네트워크 구성 및 노드 특성 추출
     - Flower 기반 연합 학습 구조로 클라이언트 노드 간 파라미터 통합

  2. **데이터 전처리 및 실험 설계**
     - IEEE-CIS Fraud Detection Dataset 기반 그래프 데이터 생성
     - 클라이언트 노드 분할, 그래프 저장, anomaly 라벨링 처리

  3. **성능 평가 및 분석**
     - Precision, Recall, F1-score, AUC 기반 이상거래 탐지 성능 검증

- **기술 스택**:  
  ![Python](https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white)  
  ![Flower](https://img.shields.io/badge/flower-FED700?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0naHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmcnIHdpZHRoPScxMCcgaGVpZ2h0PScxMCc+PHJlY3Qgd2lkdGg9JzEwMCUnIGhlaWdodD0nMTAwJScgZmlsbD0nI0ZFRDcwMCcvPjwvc3ZnPg==)  
  ![PyTorch Geometric](https://img.shields.io/badge/pytorch%20geometric-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)

- [📎 프로젝트 상세 설명 보기](https://github.com/seonmin8284/fraud_gnn_federated)

</details>

</br>

## 4. EXAONE-Deep-RAG-Ollama: FastAPI와 FAISS를 활용한 RAG 시스템
<details>
<summary>펼치기</summary>

- **개발기간**: 2025.03 ~

- **작업 범위**:  
  보험 상품요약서를 PDF로 업로드하고, 내용을 벡터화하여 검색한 뒤  
  Ollama 기반의 EXAONE-DEEP LLM을 통해 정확한 응답을 생성하는 RAG 시스템 구축

- **역할 및 업무**:
  1. **PDF 문서 처리**
     - PyPDF2를 이용해 PDF 텍스트 추출
     - 슬라이딩 윈도우 방식으로 문단 청크 생성

  2. **벡터 임베딩 및 검색**
     - `jhgan/ko-sroberta-multitask` 모델로 문장 임베딩
     - FAISS를 이용해 벡터 인덱싱 및 유사도 기반 문서 검색

  3. **RAG 시스템 구성**
     - 검색된 내용 기반으로 EXAONE LLM에 프롬프트 전달
     - 사용자 질의에 대한 근거 기반 응답 생성

  4. **API 서비스화**
     - FastAPI로 `/query` 엔드포인트 구현
     - 로컬 Ollama EXAONE 서버와 통신

- **기술 스택**:  
  ![Python](https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white)  
  ![FastAPI](https://img.shields.io/badge/fastapi-009688?style=for-the-badge&logo=fastapi&logoColor=white)  
  ![FAISS](https://img.shields.io/badge/faiss-005571?style=for-the-badge)  
  ![Ollama](https://img.shields.io/badge/ollama-7A3E9D?style=for-the-badge)  
  ![SentenceTransformer](https://img.shields.io/badge/sentencetransformer-FF6F00?style=for-the-badge)

- [📎 프로젝트 상세 설명 보기](https://github.com/seonmin8284/exaone-rag-ollama)

</details>

</br>

## 5. Kafka + Spark + Airflow를 활용한 실시간 뉴스 키워드 분석 파이프라인
<details>
<summary>펼치기</summary>

- **개발기간**: 2025.04  
- **작업 범위**:  
  Kafka로 뉴스 데이터를 스트리밍하고, Spark로 키워드 분석을 수행하며, Airflow로 파이프라인을 스케줄링하는 **데이터 엔지니어링 실습 프로젝트**

- **역할 및 업무**:
  1. **Kafka 프로듀서 개발**
     - 실시간 뉴스 API or 더미 데이터를 Kafka 토픽으로 전송
     - `kafka_news_producer.py` 구현

  2. **Spark 스트리밍 처리**
     - Kafka에서 받은 메시지를 실시간 분석
     - 주요 키워드 필터링 및 콘솔 출력

  3. **Airflow DAG 설계**
     - `news_pipeline_dag.py`로 뉴스 파이프라인 자동 스케줄링
     - ETL 흐름 제어 가능하게 DAG 구성

  4. **도커 환경 구성**
     - `docker-compose.yml`을 통해 Kafka, Spark, Airflow를 로컬에서 컨테이너 기반 실행
     - 서비스 간 의존성 관리 및 재현 가능한 환경 구현

- **기술 스택**:  
  ![Kafka](https://img.shields.io/badge/kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)  
  ![Apache Spark](https://img.shields.io/badge/spark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white)  
  ![Airflow](https://img.shields.io/badge/apache%20airflow-017CEE?style=for-the-badge&logo=apacheairflow&logoColor=white)  
  ![Docker](https://img.shields.io/badge/docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)  
  ![Python](https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white)

- [📎 프로젝트 상세 설명 보기](https://github.com/seonmin8284/kafka_spark_airflow)

</details>

</br>


## 6. 콘텐츠 추천 시스템을 활용한 GPT 기반 대화형 팟캐스트(PODLY) 
<details>
<summary>펼치기</summary>
  
>
> - 개발기간 : 2024.10
> - 작업 범위 : 컨텐츠 추천 시스템 개발, RAG를 활용한 LLM 기반 챗봇 구현, STT 및 TTS 구현, 모바일 플랫폼 개발 
> - 역할 및 업무: 모바일 크로스플랫폼 앱 프론엔드 제작
>   
>   (1) UI/UX 설계
>   
>   (2) 모바일 크로스플랫폼 제작
>   1) 맞춤형 컨텐츠 재생 뮤직 플레이어 구현
>   2) 토큰 기반 자연어 스트림 UX 챗봇과 TTS 음성 출력 구현
>   3) 유튜브 API 연결로 인기 컨텐츠 페이지 구현
>   4) 검색, 좋아요, 공유하기 등 세부 기능 구현  
> - Skill : <img src="https://img.shields.io/badge/flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white">
> 
> [프로젝트 상세 설명](https://github.com/seonmin8284/podly)

</details>

<br />


## 7. ~~(미완성)stable diffusion, TTS(Text to Speach AI)를 활용한 AI 가상인간 영상 제작~~
<details>
<summary>펼치기</summary>
  
>
> - 개발기간 : 2024.02-2024.05
> - 작업 범위 : 음성 모델 제작, 가상 인물 영상 제작, 립싱크 합성
> - 역할 및 업무:
>   
>   (1) ComfyUI를 활용한 stable diffusion 기반 영상 제작
>   
>   (2) tortoise 모델 학습을 통한 TTS 모델 제작
>   
> - Skill : <img src="https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white"> 
> 
> [프로젝트 상세 설명](https://github.com/seonmin8284/virtualHuman)

</details>

<br />



## 8. 전세 사기 예방을 위한 블록체인 기반 OCR 활용 부동산 계약 시스템
<details>
<summary>펼치기</summary>
  
>
> - 개발기간 : 2022.06-2022.08
> - 작업 범위 : 블록체인 스마트 컨트랙트 기반 부동산 계약 자동화 시스템 설계, 분산 신원 확인을 통한 참여자 검증 설계, Tesseract OCR 기술을 활용하여 기존 부동산 관련 문서 분석 및 정보 추출 구현, 공공 데이터 API를 활용한 위험 감지 및 변동 사항 알림 시스템 구현
> - 역할 및 업무:
>   
>   (1) 서비스 기획 총괄
>   1) 부동산 전세사기 문제 분석 및 시장 조사
>   2) 프로젝트의 전반적인 블록체인 AI 서비스 기획 및 방향 설정
>      
>   (2) Tesseract OCR 기반 부동산 문서 내 글자 인식 구현
>   
>   (3) 공공 데이터 API를 활용 Flask 서버 및 전체 프로토타입 구현
> 
> - Skill : <img src="https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white"> 
> 
> [부동산 문서 Tesseract OCR 설명 + 프로젝트 상세 설명](https://github.com/seonmin8284/realEstateOCR)

</details>

<br />

## ~~9. 미완성 협업용 영화 스튜디오 공유 모바일 플랫폼~~
<details>
<summary>펼치기</summary>
  
>
> - 개발기간 : 2022.07.07-09.02
> - 작업 범위 : 
> - 역할 및 업무:
> (1) ㄹㅇㄹㅇ
> (2) ㄹㄴㄷㄷ
> - Skill : <img src="https://img.shields.io/badge/flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white">
> 
> ~~[프로젝트 상세 설명](https://github.com/seonmin8284/nawaPJ)~~
</details>

<br />

## ~~10. 미완성 테니스 동아리 회원 전용 테니스장 예약 모바일 플랫폼~~
<details>
<summary>펼치기</summary>
  
>
> - 개발기간 : 2022.07.07-09.02
> - 작업 범위 : 
> - 역할 및 업무:
> (1) ㄹㅇㄹㅇ
> (2) ㄹㄴㄷㄷ
> - Skill : <img src="https://img.shields.io/badge/flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white">
>   
> ~~[프로젝트 상세 설명](https://github.com/seonmin8284/nawaPJ)~~
</details>
<br />

## ~~11. 미완성  NAWA 재활용 종이컵 스타트업 홈페이지 제작~~
<details>
<summary>펼치기</summary>
  
>
> - 개발기간 : 2022.07.07-09.02
> - 작업 범위 : 
> - 역할 및 업무: 
> (1) ㄹㅇㄹㅇ
> (2) ㄹㄴㄷㄷ
> - Skill : <img src="https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white"><img src="https://img.shields.io/badge/css-1572B6?style=for-the-badge&logo=css3&logoColor=white"><img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
> 
> ~~[프로젝트 상세 설명](https://github.com/seonmin8284/nawaPJ)~~
</details>

<br />


## 12. 제조업 노동자 근골격계 부담요인 예방 인공지능 데이터 구축
<details>
<summary>펼치기</summary>
  
>
> - 개발기간 : 2022.07.07-09.02
> - 작업 범위 : YOLOv5를 활용한 객체 검출, HRNet 기반의 자세 추정, EfficientNet을 이용한 다중 라벨 분류, 인간공학적 평가 기법을 적용한 자세 분석, 그리고 EfficientNet-Lite를 활용한 모바일 환경 최적화까지의 AI 모델 개발 및 응용
> - 역할 및 업무: 
>
>   (1) AI 서비스 기획 총괄
>   1) 프로젝트의 전반적인 AI 서비스 기획 및 방향 설정
>   2) 각 Task 간 연계성을 고려한 서비스 설계 및 성능 최적화
>   
>   (2) YOLOv5 기반 객체 검출 담당
>   1) YOLOv5s를 활용하여 데이터 전처리 및 객체 검출 모델 학습, Task 02에서 활용할 Cropped 이미지 생성
>   
>   (3) 모바일 제작 담당
>   1) Flutter를 활용한 UI/UX 설계 및 구현
>   2) EfficientNet-Lite 기반 모바일 애플리케이션 개발 및 최적화
>   3) AI 모델을 모바일 환경에 배포 및 성능 테스트 진행

> - Skill : <img src="https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white"> <img src="https://img.shields.io/badge/flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white">
> 
> 
> [프로젝트 상세 설명](https://github.com/seonmin8284/skeleton_Vision/tree/main)
</details>

<br />


<div align=center><h1>📚 LANGUAGE</h1></div>
<div align=center>
<img src="https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white"> 
  <img src="https://img.shields.io/badge/java-007396?style=for-the-badge&logo=java&logoColor=white"> 
  <br>
  <h1>:bulb: ML/DL</h1>
   <img src="https://img.shields.io/badge/tensorflow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white"> 
  <img src="https://img.shields.io/badge/pytorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white"> 
   <img src="https://img.shields.io/badge/opencv-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white"> 
  <br>
  <h1>:computer: WEB</h1>
  [포트폴리오_1](https://github.com/seonmin8284/nawaPJ)<br><br>
   <img src="https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white"> 
  <img src="https://img.shields.io/badge/css-1572B6?style=for-the-badge&logo=css3&logoColor=white"> 
  <img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
  <br>
  <h1>:iphone: MOBILE</h1>
  [포트폴리오_1](https://play.google.com/store/apps/details?id=com.tennis.tennis)<br><br>
    <img src="https://img.shields.io/badge/flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white">
  <h1>:cloud:SERVER</h1>
   <img src="https://img.shields.io/badge/Google Cloud-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white">
    <img src="https://img.shields.io/badge/firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=white">
<h1>DATABASE</h1>
  <img src="https://img.shields.io/badge/mysql-4479A1?style=for-the-badge&logo=mysql&logoColor=white">
  <h1>REST API</h1>
  <img src="https://img.shields.io/badge/flask-000000?style=for-the-badge&logo=flask&logoColor=white">
  
</div>

