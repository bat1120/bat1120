<h1 align="center">안녕하세요, AI 엔지니어를 지망하는 홍찬영입니다 👋</h1>

<p align="center">
  <b>LLM · 컴퓨터 비전 · NLP</b>를 폭넓게 다루며,<br/>
  데이터 수집부터 모델링·RAG·서비스 구현까지 <b>직접 만들어보며</b> 성장하고 있습니다.<br/>
  "정확도를 올렸다"를 <b>정량 지표로 증명</b>하는 습관을 중요하게 생각합니다.
</p>

<p align="center">
  <a href="mailto:bat981120@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white"/></a>
</p>

---

## 🙋‍♂️ About Me

- 🤖 멀티에이전트 + RAG 기반 **AI 출점 시뮬레이터**(팀 프로젝트)에서 데이터·DB·RAG를 담당 — 법률 RAG 검색 정확도 **Hit@10 62% → 100%** 개선
- 📰 **Self-RAG 뉴스 에이전트**를 개인 프로젝트로 구현 — LangGraph, 임베딩 캐시, critic LLM 재시도, LLM-as-judge 평가
- 👁 자세 추정 · 객체 탐지 · OCR · LLM을 통합한 **AI 코치 앱** 등 비전/언어 전반을 폭넓게 실습
- 🌱 논문·새 모델을 직접 코드로 재현하고, 재현 가능한 실험으로 개선을 증명하는 것을 좋아합니다

---

## 🛠 Tech Stack

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)

**AI / ML**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)

**Data / MLOps**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)

<!-- 실제로 다뤄본 것만 남기고, 안 써본 건 지우세요. 면접에서 배지에 적힌 건 다 질문받을 수 있습니다. -->

---

## 📌 Projects

### 🏪 AI 출점 시뮬레이터 — 프랜차이즈 매출·폐업·법률 리스크 예측
프랜차이즈 본부 영업팀을 위해, 서울 공공데이터를 기반으로 입지별 사업성을 예측하는 AI 시스템입니다.
- **문제**: 신규 점포 출점 시 매출·폐업·법률 리스크를 데이터로 사전 검증
- **접근**: **LangGraph 병렬 멀티에이전트** 파이프라인 + **TCN · LightGBM 앙상블** 예측 + **SHAP** 해석 + **RAG** 기반 법률 리스크 분석
- **결과**: 마포구 16개 동 × 10개 업종의 매출/폐업/법률 리스크를 12개월 예측 (서울 19종 이상 공공데이터 활용)
- **기술**: Python, LangGraph, LightGBM, TCN, SHAP, RAG
- 🔗 [Repository](https://github.com/Himidea-AI/Final_Project)
<!-- TODO: 본인이 맡은 역할(담당 모듈)과 정량 지표(예: 예측 정확도/MAE)를 추가하면 훨씬 강력해집니다. -->

### 📰 Self-RAG 뉴스 큐레이션 에이전트
멀티 소스 뉴스를 수집·재랭킹하고, critic LLM이 결과 품질을 채점해 부족하면 다시 검색하는 Self-RAG 에이전트입니다.
- **접근**: LangGraph 병렬 멀티소스 수집 + OpenAI 임베딩 재랭킹 + critic 재시도(Self-RAG) + ReAct 에이전트
- **기술**: Python, LangGraph, OpenAI, Flask, Discord
- 🔗 [Repository](https://github.com/HiMedia13/ai_news_summarizer)

### 🎩 마술 영상 분석기 (magic-analyzer)
카드·동전 마술 영상에서 손을 추적해 '수상한 순간'(팜·전달·급동작)을 타임라인으로 짚어주는 분석 도구입니다.
- **접근**: MediaPipe 손 추적 + 신호 점수화/NMS 봉우리 탐지 + ReAct 도구 호출 에이전트(OpenAI 비전) + 기법 라이브러리 매칭(RAG)
- **기술**: Python, MediaPipe, OpenCV, LangGraph, OpenAI, Flask
- 🔗 [Repository](https://github.com/HiMedia13/magic-analyzer)

### 📸 사진 자동 분류 PWA (photo-classifier-pwa)
휴대폰 사진을 AI로 설명·임베딩한 뒤 군집화해 자동으로 앨범을 만들어주는 PWA입니다.
- **접근**: gpt-4o Vision 설명 → text-embedding-3-small 임베딩 → HDBSCAN 자동 군집 → 클러스터 이름 자동 부여
- **기술**: Python, Flask, OpenAI Vision, HDBSCAN, PWA
- 🔗 [Repository](https://github.com/bat1120/photo-classifier-pwa)

### 🧪 AI 기능 통합 실습 — LLM · 컴퓨터 비전 · OCR
여러 AI 기능을 직접 구현하며 분야별로 익힌 개인 실습입니다.
- **LLM**: 챗봇, 이메일 자동 작성/재작성, Gemini · Ollama 연동
- **컴퓨터 비전**: 이미지 분류, 객체 탐지, 얼굴 인식, 자세(pose) 추정 / **OCR**: 텍스트 추출·번역
- **기술**: Python, OpenCV, LLM API
- 🔗 [Repository](https://github.com/bat1120/ai-experiments)


---

## 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=bat1120&show_icons=true&theme=default&hide_border=true&count_private=true" height="165"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=bat1120&layout=compact&theme=default&hide_border=true&langs_count=8" height="165"/>
</p>

---

<p align="center"><i>읽어주셔서 감사합니다. 함께 성장할 기회를 찾고 있습니다.</i></p>
