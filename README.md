<h1 align="center">홍찬영 · Hong Chan Young</h1>

<p align="center">
  <b>LLM 에이전트 엔지니어</b> &nbsp;|&nbsp; Multi-Agent · RAG · Agentic Workflow
</p>

<p align="center">
  반복되는 일을 <b>에이전트에게 넘기는</b> 데 집중합니다.<br/>
  LangGraph로 멀티에이전트를 엮고, RAG로 근거를 붙이고, critic 루프로 스스로 고치게 만듭니다.<br/>
  "정확도를 올렸다"를 <b>숫자로 증명</b>하고, 모델만큼이나 <b>안 죽는 서비스 구조</b>를 신경 씁니다.
</p>

<p align="center">
  <a href="mailto:bat981120@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white"/></a>
  <img src="https://img.shields.io/badge/Base-Seoul,_KR-555?style=flat-square&logo=googlemaps&logoColor=white"/>
</p>

---

## 🤖 What I Build

- 🧩 **멀티에이전트** — LangGraph로 역할을 나눈 에이전트를 병렬·협업시켜 복잡한 업무를 분해해 처리
- 🔁 **Self-RAG / 반성 루프** — critic LLM이 결과를 채점하고, 부족하면 쿼리를 다시 써서 재검색
- 🛠 **Tool-calling(ReAct)** — LLM이 직접 도구(검색·비전·DB)를 호출할지 스스로 판단하는 파이프라인
- 🧱 **고도화된 RAG** — Parent-Child 청킹·임베딩 재랭킹으로 검색 품질을 정량적으로 끌어올림
- 🛡 **폴백 설계** — 모델·외부 API가 죽어도 대체 경로로 넘어가 서비스가 멈추지 않게 구성

> 회사에서 **LangChain·LangGraph 문서 자동화 에이전트**를 만들어 문서 작업 시간을 **약 50% 단축**했고,
> 퇴근 후에도 에이전트를 직접 만들어 보며 어디까지 자동화되는지 확인하는 편입니다.

---

## 🛠 Tech Stack

**LLM / Agent**

![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langgraph&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white)
![RAG](https://img.shields.io/badge/RAG-0A7E07?style=flat-square&logo=databricks&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)
![Claude](https://img.shields.io/badge/Claude-D97757?style=flat-square&logo=anthropic&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)

**ML / Vision**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)

**Backend / Infra**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

<sub>※ 실제로 다뤄본 것만 남겼습니다. 면접에서 배지에 적힌 건 다 질문받을 수 있어서요.</sub>

---

## 📌 Featured Projects

### 🏪 AI 출점 시뮬레이터 — 멀티에이전트 입지 사업성 예측 <sub>(팀)</sub>
신규 점포의 매출·폐업·법률 리스크를 데이터로 미리 검증해 주는 시스템.
- **에이전트 구조** — LangGraph **병렬 멀티에이전트** 파이프라인이 예측·해석·법률 검토를 나눠 수행
- **내 역할** — 데이터 파이프라인 · DB · 법률 RAG 담당
- **결과** — 법률 RAG 검색 **Hit@10 62% → 100%**, 마포구 16개 동 × 10개 업종을 12개월 예측
- `LangGraph` `RAG` `LightGBM` `TCN` `SHAP` `Python`
- 🔗 https://github.com/Himidea-AI/Final_Project

### 📰 Self-RAG 뉴스 큐레이션 에이전트 <sub>(개인)</sub>
여러 출처의 뉴스를 모아 재랭킹하고, **critic LLM이 결과를 채점해 부족하면 다시 검색**하는 반성형 에이전트.
- **에이전트 구조** — LangGraph 멀티소스 병렬 수집 → 임베딩 재랭킹 → critic 재시도(Self-RAG) → ReAct 도구 호출
- **결과** — Flask 웹과 Discord 봇 양쪽으로 자동 브리핑
- `LangGraph` `Self-RAG` `ReAct` `OpenAI` `Flask` `Discord`
- 🔗 https://github.com/HiMedia13/ai_news_summarizer

### 🎩 마술 영상 트릭 분석 에이전트 <sub>(개인)</sub>
마술 영상에서 '수상한 순간'을 짚고, **에이전트가 직접 그 장면을 들여다보며** 기법을 추론·설명.
- **에이전트 구조** — 신호 탐지(MediaPipe·YOLO) → LangGraph **ReAct 도구 호출** 에이전트가 gpt-4o Vision으로 구간 분석
- **포인트** — 비밀을 단정하지 않고 *의심 구간*만 골라 사람이 다시 보게 돕는 보조 도구로 설계
- `LangGraph` `ReAct` `OpenAI Vision` `MediaPipe` `YOLOv8`
- 🔗 https://github.com/HiMedia13/magic-trick-analyzer

### 📖 AI 동화 만들기 — LLM 오케스트레이션 <sub>(교육 미니프로젝트 · 팀)</sub>
아이가 그린 그림으로 AI가 동화 스토리·배경 이미지·음성을 만들어 한 권으로 완성해 주는 웹앱.
- **내 역할** — AI 스토리 생성 + 배경 이미지 생성
- **에이전트/안정성** — 스토리(Gemini→Claude)·이미지(로컬 LCM→Pollinations) **폴백 체인**으로 외부 API가 죽어도 멈추지 않게 설계
- `LLM Orchestration` `Gemini` `Claude` `Flask` `LCM-DreamShaper` `CLOVA Voice`
- 🔗 https://github.com/first-mini-project/mini-project

<sub>그 외 — 📸 <a href="https://github.com/HiMedia13/photo-classifier-pwa">photo-classifier-pwa</a> (gpt-4o Vision + HDBSCAN 사진 자동 분류 PWA) 등</sub>

---

## 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=bat1120&show_icons=true&theme=default&hide_border=true&count_private=true&include_all_commits=true" height="165"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=bat1120&layout=compact&theme=default&hide_border=true&langs_count=8" height="165"/>
</p>

<sub>※ 프로젝트가 여러 계정(<code>bat1120</code> · <code>HiMedia13</code> · <code>Himidea-AI</code>)에 흩어져 있어, 위 통계는 활동의 일부만 보여줍니다.</sub>

---

<p align="center"><i>읽어주셔서 감사합니다 — 에이전트로 사람의 시간을 아끼는 일을 함께 하고 싶습니다. 🚀</i></p>
