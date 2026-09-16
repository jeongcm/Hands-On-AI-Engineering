<p align="center">
  <a href="https://aiengineering.beehiiv.com/">
    <img src="assets/theaiengineering_logo.jpeg" alt="Hands-On AI Engineering 배너" width="150">
  </a>
</p>
<div align="center">

# 🚀 Hands-On AI Engineering

[![라이선스: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PR 환영](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

</div>

언어 모델, 멀티모달 모델, OCR 시스템, RAG 파이프라인, AI 에이전트 등 다양한 모달리티를 아우르는 실용적이고 프로덕션 활용을 고려한 AI 프로젝트 모음입니다. 각 프로젝트는 학습과 실험을 통해 실제로 활용할 수 있는 AI 애플리케이션을 만드는 데 도움이 되도록 설계되었습니다.

## 📋 목차

- [🎯 이 저장소를 활용하는 이유](#-이-저장소를-활용하는-이유)
- [🗂️ 프로젝트 분류](#️-프로젝트-분류)
- [🤝 기여하기](#-기여하기)
- [📜 라이선스](#-라이선스)

---

## 🎯 이 저장소를 활용하는 이유

- **실습 중심 학습**: 각 프로젝트에 전체 코드, 설정 방법, 문서가 포함되어 있습니다.
- **프로덕션 활용 고려**: 모범 사례를 따르며 실제 환경에 맞게 적용할 수 있도록 구성되어 있습니다.
- **다양한 활용 사례**: RAG 시스템부터 멀티 에이전트 워크플로와 특화 애플리케이션까지 다룹니다.
- **다양한 모델 제공업체**: OpenAI, Anthropic, Google 및 오픈 소스 모델을 활용합니다.
- **활발한 커뮤니티**: 정기적인 업데이트와 새로운 프로젝트 추가가 이루어집니다.

---

## 🗂️ 프로젝트 분류

### 🤖 AI 에이전트

다양한 자동화 작업을 수행하는 지능형 AI 에이전트입니다.

- [**메모리를 갖춘 멀티 에이전트 리서치 어시스턴트**](./ai_agents/research_assistant_with_memory) — 기획, 조사, 작성, 비평 에이전트가 공유 [Actian VectorAI DB](https://www.actian.com/databases/vectorai-db/) 메모리 계층을 통해 협업합니다. PDF, 논문, 매뉴얼, 녹취록에서 출처를 인용한 답변을 검색하고, 비평 에이전트의 피드백 루프로 자체 평가하며, 조사 결과를 세션 간에 유지합니다. Ollama와 BGE 임베딩을 사용해 완전히 로컬에서 실행됩니다.
- [**멀티 에이전트 금융 분석가**](./ai_agents/multi_agent_financial_analyst) — 전문 에이전트 팀이 종합적인 금융 분석을 수행합니다.
- [**FinAgent**](./ai_agents/finagent) — 주식 시장 분석과 인사이트를 제공하는 금융 어시스턴트 에이전트입니다.
- [**일일 AI 뉴스 요약**](./ai_agents/daily-news-digest) — Karpathy가 선정한 기술 블로그 92곳의 일일 요약을 매일 아침 Telegram으로 자동 전달합니다. MiniMax M2.7이 최근 24시간 동안의 기사를 평가해 가장 중요한 소식 3개를 선정합니다.
- [**에이전트 기반 폼 작성 도우미**](./ai_agents/agentic-form-filler) — Landing AI로 레이아웃을 분석하고 MiniMax M2.7으로 여러 차례 대화하며 정보를 수집해 폼을 작성하는 에이전트입니다.
- [**AI 여행 계획 에이전트**](./ai_agents/ai_travel_planning_agent) — 자연어 요청 하나를 항공편, 호텔, 일자별 일정을 포함한 완전한 여행 계획으로 만드는 멀티 에이전트 여행 플래너입니다.
- [**경쟁사 분석 에이전트**](./ai_agents/competitive_intelligence_agent) — 자사 비즈니스 맥락에서 경쟁사를 분석해 전략적인 영업용 경쟁 대응 자료를 생성합니다.
- [**멀티 에이전트 리서치 어시스턴트(AG2)**](./ai_agents/multi_agent_research_assistant_ag2) — AG2를 사용하는 멀티 에이전트 조사 파이프라인입니다. 세 명의 전문가가 협업해 주제를 조사하고 구조화된 보고서를 작성합니다.
- [**자기 성찰형 에이전트 RAG**](./ai_agents/agentic_rag_system) — 검색한 맥락을 평가하고 필요하면 질의를 재작성하며, 맥락이 검증을 통과한 경우에만 답변을 생성하는 LangGraph RAG 시스템입니다.
- [**에이전트 기반 SQL 검색**](./ai_agents/agentic_sql_search) — Gemma 4 기반 자연어-SQL 에이전트로, 전자상거래 데이터베이스에 대한 쿼리를 작성·실행하고 설명합니다.
- [**주식 포트폴리오 분석가**](./ai_agents/stock_portfolio_analyst) — Agno와 DeepSeek-V4-Flash로 만든 포트폴리오 분석 에이전트입니다. YFinance로 실시간 시장 데이터를 가져와 손익, 집중 위험, 리밸런싱 제안을 담은 보고서를 생성합니다.
- [**Eagle Eye**](./ai_agents/eagle_eye) — OpenClaw와 Telegram을 사용하는 GitHub PR 리뷰 에이전트입니다. GitHub MCP로 변경 내역을 가져와 심각도 평가를 포함한 구조화된 코드 리뷰를 수행하고, 사용자 승인 후 피드백을 게시합니다.
- [**CartMate — AI 고객 지원 에이전트**](./ai_agents/ai_customer_support_agent) — Mem0와 Mistral Small 4로 만든 메모리 기반 전자상거래 지원 에이전트입니다. 고객을 기억하고 이전에 중단된 지점부터 대화를 이어갑니다.
- [**멀티 에이전트 코딩 어시스턴트**](./ai_agents/multi_agent_coding_assistant) — Mistral Small 4와 LangChain 기반의 4단계 코딩 파이프라인입니다. 기획, 코딩, 리뷰 에이전트가 협업해 완성도 높은 최종 구현을 만듭니다.
- [**스타트업 분석가**](./ai_agents/startup_analyst) — MiniMax M2.5 기반 스타트업 실사 에이전트입니다. Firecrawl로 회사 웹사이트를 수집하고 시장 내 입지, 재무, 팀, 위험 요인을 담은 투자 검토용 보고서를 작성합니다.
- [**리서치 팀**](./ai_agents/research_team) — MiniMax M2.5 기반 멀티 에이전트 조사 시스템입니다. Seek는 웹을 검색하고 Scout는 내부 문서를 탐색하며, 팀 리더가 결과를 종합해 구조화된 보고서를 작성합니다.
- [**GitHub 분석 에이전트**](./ai_agents/github_intelligence_agent) — Gemini 3 Flash와 GitHub 공식 MCP 서버 기반의 GitHub 조사 에이전트입니다. 저장소, 기여자, 이슈, 코드베이스에 관해 질문할 수 있습니다.
- [**Smolagents 코드 에이전트**](./ai_agents/smolagents_code_agent) — Mistral Small 4와 HuggingFace smolagents 기반의 에이전트형 작업 실행기입니다. DuckDuckGo와 Wikipedia를 활용하며 각 단계에서 Python 코드를 작성하고 실행합니다.
- [**에이전트 탐색 에이전트**](./ai_agents/agent_discovery_agent) — 하나의 자연어 인터페이스로 NANDA, MCP, Virtuals Protocol, A2A, ERC-8004의 AI 에이전트를 검색하고 비교합니다. Gemini 3 Flash를 사용합니다.
- [**Cal 일정 관리 에이전트**](./ai_agents/cal_scheduling_agent) — 자연어로 Cal.com 예약을 관리하는 대화형 일정 어시스턴트입니다. 시간대를 자동으로 처리하며 예약 생성, 변경, 취소 및 예약 가능 시간 확인을 지원합니다.
- [**Hacker News 뉴스레터 에이전트**](./ai_agents/hacker_news_newsletter_agent) — Hacker News의 최신 소식 10개를 가져오고 Trafilatura로 기사 본문을 수집한 뒤, Gemma 4로 구조화된 HTML 뉴스레터를 만들어 Gmail SMTP로 이메일을 보냅니다.
- [**호텔 검색 에이전트**](./ai_agents/hotel_finder_agent) — Orq.ai를 통한 qwen3.6-flash와 Trivago MCP Server 기반의 대화형 호텔 검색 에이전트입니다. 위치, 날짜, 투숙객 수, 가격대, 성급, 편의시설로 검색할 수 있습니다.
- [**마케팅 전략 에이전트**](./ai_agents/marketing_strategy_agent) — 멀티 에이전트 마케팅 캠페인 생성기입니다. Serper 웹 검색을 활용하는 시장 분석가, 전략 담당자, 크리에이티브 디렉터가 순차적으로 실행되어 시장 조사, 전체 전략, 캠페인용 크리에이티브 콘텐츠를 만듭니다. Orq.ai를 통해 deepseek-v4-flash를 사용합니다.
- [**브랜드 모니터**](./ai_agents/brand_monitor_agent) — 한 번의 실행으로 웹, YouTube, Twitter/X, LinkedIn의 브랜드 언급을 모니터링합니다. Scrapingdog이 플랫폼 데이터를 수집하고 DeepSeek V4 Flash가 채널별로 구조화된 분석 브리프를 작성합니다.
- [**AI 토론 에이전트**](./ai_agents/ai_debate_agent) — 두 LLM 토론자가 선택한 주제에 대해 서로 반대 입장에서 논쟁합니다. 심판이 매 차례 점수를 매기고 승자를 결정합니다.
- [**브라우저 자동화 에이전트**](./ai_agents/browser_automation_agent) — 자연어 지시를 받아 browser-use로 웹을 자율적으로 탐색하며 작업을 완료합니다.
- [**문서 질의응답 에이전트**](./ai_agents/documentation_qna_agent) — URL로 제공한 문서를 대상으로 대화할 수 있습니다. Fetch MCP와 NVIDIA NIM의 DeepSeek V4 Flash를 사용합니다.
- [**채용 공고 작성 에이전트**](./ai_agents/job_posting_agent) — NVIDIA NIM의 DeepSeek V4 Flash를 사용해 회사 이름과 직무에 맞춘 채용 공고를 생성합니다.
- [**LangChain 데이터 에이전트**](./ai_agents/langchain_data_agent) — 대화형 Streamlit 채팅 인터페이스에서 일상적인 영어로 Chinook SQLite 데이터베이스를 조회합니다.
- [**여행 플래너 에이전트**](./ai_agents/travel_planner_agent) — 요청 하나로 날씨, 예산, 준비물 목록, 일자별 일정을 다루는 AI 여행 계획 어시스턴트입니다.
- [**개인 재무 에이전트**](./ai_agents/personal_finance_agent) — 은행 거래 내역 CSV를 업로드하면 거래를 자동 분류하고 지출에 관한 자연어 질문에 답합니다. Orq.ai 기반의 LangChain 도구 호출 에이전트를 사용하며 데이터를 SQLite에 영구 저장합니다.
- [**오프라인 의료 에이전트**](./ai_agents/offline_medical_agent) — 외딴 지역의 진료소와 야전 병원에서 임상 프로토콜을 조회하기 위한 완전 오프라인 에이전트형 RAG 시스템입니다.
- [**고객 문의 분류·해결 에이전트**](./ai_agents/customer_query_routing_agent) — 접수된 지원 문의를 적절한 부서로 전달하고, [Actian VectorAI DB](https://www.actian.com/databases/vectorai-db/)를 로컬 영구 메모리 및 검색 계층으로 활용해 근거 기반 답변을 생성합니다.
- [**이메일 자동 응답기**](./ai_agents/email_auto_responder) — IMAP으로 읽지 않은 Gmail 메시지를 읽고, GLM-5.1 기반 CrewAI 에이전트로 의도를 분류하며, Streamlit 대시보드에서 업무용 답장 초안을 작성합니다.
- [**LLM 농업 봇**](./ai_agents/llm_agri_bot) — Mistral 기반 LangChain 도구 호출 에이전트를 사용해 작물 건강, 날씨, 해충, 파종 시기에 관한 질문에 답하는 농업 어시스턴트입니다.
- [**근거 기반 문서 에이전트**](./ai_agents/grounded_document_agent) — 긴 PDF에 대해 질문하면 정확한 출처 페이지를 인용한 답변을 제공합니다. LlamaParse가 문서를 파싱하고, 검색과 답변 생성은 Ollama에서 로컬로 실행됩니다.
- [**자기 발전형 코드 리뷰 에이전트**](./ai_agents/self_evolving_code_review_agent) — 모델을 재학습하지 않고 엔지니어의 피드백에서 팀 규칙을 학습하는 코드 리뷰어입니다. LangGraph와 Actian VectorAI DB를 사용해 메모리를 영구 저장합니다.
- [**TrueForge 웹 리서치 브리프 생성기**](./ai_agents/trueforge_web_research_briefer) — 오픈 소스 TrueForge 하네스 기반 웹 조사 에이전트입니다. 해당 차례의 작업을 계획하고 MCP로 웹을 검색한 뒤 병렬 하위 에이전트에 작업을 분배해 출처가 명시된 한 페이지 브리프를 작성합니다.
- [**심층 리서치 어시스턴트**](./ai_agents/deep_research_assistant) — LangChain Deep Agents로 구현하고 Liner Web Search API로 근거를 확보해, 질문에 출처를 충실히 인용한 답변을 제공하는 조사 에이전트입니다.
- [**Devable 리서치 에이전트**](./ai_agents/devable_research_agent) — AI 엔지니어링 관련 동향을 수집하고 주요 항목의 순위를 매긴 뒤 구조화된 Slack 요약을 전달하는 예약 실행형 3단계 파이프라인입니다.
- [**Instagram 게시물 제작 팀**](./ai_agents/instagram_post_crew) — 주제를 Instagram 콘텐츠 패키지로 변환하는 CrewAI 파이프라인입니다. 트렌드 분석, 여러 버전의 캡션, 이미지 프롬프트, 권장 게시 시간을 제공합니다.

### 📸 OCR

시각 데이터와 문서에서 구조와 의미를 추출합니다.

- [**AI 영수증·지출 추적기**](./OCR/receipt_expense_tracker) — 영수증 사진에서 구조화된 데이터를 추출하고 로컬 SQLite 장부로 지출을 추적합니다. llama-cpp-python을 통해 Gemma 4 E2B의 비전 기능을 사용합니다. 최초 실행 이후에는 완전히 오프라인으로 동작합니다.
- [**이미지 구조화 데이터 추출기**](./OCR/image_to_structured_data) — Mistral Large 3와 Instructor를 사용해 이미지를 검증된 구조화 JSON으로 변환합니다.
- [**LaTeX 수식 OCR**](./OCR/latex_formula_ocr) — 로컬 비전-언어 모델로 이미지와 PDF에서 수식을 추출해 LaTeX로 변환합니다.
- [**의료 처방전 디지털화 도구**](./OCR/medical_prescription_digitizer) — Mistral Large 3로 손글씨 또는 인쇄된 처방전을 구조화된 데이터로 변환하고, RxNorm을 통해 약물명을 실시간으로 검증합니다.

### 🎧 오디오

오디오 이해와 분석을 위한 프로젝트입니다.

- [**음악 탐색기**](./audio/music_explorer) — Gemini 3 Flash로 오디오 파일이나 YouTube 동영상에 대해 대화합니다. 음성 전사, 감정 분석, 악기 식별, 타임스탬프별 분석을 요청할 수 있습니다.
- [**다국어 오디오 번역기**](./audio/multilingual_audio_translator) — 다양한 언어의 오디오를 업로드하거나 녹음하면 faster-whisper로 전사하고 Gemini로 번역한 뒤 Kokoro TTS로 합성 음성을 재생합니다.
- [**고객 지원 음성 에이전트**](./audio/customer_support_voice_agent) — 고객 지원 전화를 받는 음성 AI 에이전트입니다. Telnyx AI Assistant Builder와 매 통화에 실시간 맥락을 주입하는 FastAPI 웹훅으로 구현되었습니다.

### 🎬 멀티모달

비전, 비디오, 언어 모델을 결합하는 프로젝트입니다.

- [**GLM-OCR Pro**](./multimodal/glm_ocr_pro) — Ollama를 통해 GLM-OCR을 사용하여 문서의 구조화된 정보를 추출하고, 이미지와 PDF를 로컬에서 서식이 적용된 Markdown으로 변환합니다.
- [**동영상 이해 에이전트**](./multimodal/video_understanding_agent) — Gemini Flash로 YouTube 동영상을 챕터, 핵심 내용, 실행 항목으로 요약합니다.
- [**멀티모달 날씨 앱**](./multimodal/multimodal_weather_app) — 지도 이미지를 업로드하면 실시간 날씨를 제공합니다. Mistral Small 4가 비전 기능으로 도시를 식별한 뒤 네이티브 도구 호출로 현재 기상 정보를 가져옵니다.
- [**멀티모달 RAG**](./multimodal/multimodal_rag) — 텍스트, URL, PDF, 이미지, 오디오, 비디오를 공통 ChromaDB 인덱스에 수집하는 RAG 시스템입니다. Gemini Embedding 2가 검색을 담당하고 Gemini 3 Flash가 근거 기반 답변을 생성하며, 미디어 소스에는 실제 파일 URI를 전달합니다.
- [**이미지 질의응답**](./multimodal/image_question_answering) — PDF를 업로드하고 페이지를 선택해 시각적 내용에 관해 질문하면, 사고 모드가 활성화된 Gemma 4가 답합니다. PyMuPDF가 각 페이지를 원본 해상도 이미지로 렌더링해 차트, 표, 그림에 근거한 추론을 지원합니다.
- [**의료 문서 파서**](./multimodal/medical_document_parser) — Gemma 4의 비전 기능으로 의료 PDF와 이미지에서 구조화된 임상 프로필을 추출합니다.

### 📚 RAG 애플리케이션

지식을 활용해 AI 애플리케이션을 강화하는 검색 증강 생성(RAG) 시스템입니다.

- [**O3-Mini·DuckDuckGo 기반 에이전트 RAG**](./rag_apps/agentic_rag_with_o3_mini_and_duckduckgo) — O3-Mini와 DuckDuckGo를 사용해 실시간 웹 검색을 수행하는 RAG 시스템입니다.
- [**Qwen·FireCrawl 기반 에이전트 RAG**](./rag_apps/agentic_rag_with_qwen_and_firecrawl) — Qwen과 FireCrawl로 웹 수집과 검색을 수행하는 RAG 시스템입니다.
- [**비전 RAG**](./rag_apps/vision_rag) — 시각 콘텐츠를 처리하고 질의하는 멀티모달 RAG 시스템입니다.
- [**ADE 기반 임상 RAG**](./rag_apps/clinical_rag_with_ade) — LandingAI ADE로 시각 정보 중심의 문서 파싱을 수행하고 Mistral Large로 근거 기반 추론을 수행하는 고정밀 임상 RAG입니다.
- [**YouTube 전사문 RAG**](./rag_apps/youtube_transcript_rag) — Whisper 음성 전사, ChromaDB 검색, Mistral Small 4를 활용해 YouTube 동영상에 대해 대화하고, 타임스탬프 링크가 포함된 답변을 제공합니다.
- [**GraphRAG 지식 시스템**](./rag_apps/graphrag_knowledge_system) — Mistral Small 4와 NetworkX로 업로드한 문서에서 로컬 지식 그래프를 구축하며, 개체 수준 질의와 주제 중심 질의를 모두 지원합니다.
- [**하이브리드 RAG 시스템**](./rag_apps/hybrid_rag_system) — 문서를 지식 그래프와 벡터 저장소에 병렬로 인덱싱합니다. Mistral Small 4가 두 검색 경로의 맥락을 결합해 질문에 답합니다.
- [**HyDE RAG**](./rag_apps/hyde_rag) — 가상 문서 임베딩(Hypothetical Document Embeddings)을 사용하는 RAG 파이프라인입니다. Gemini 3 Flash가 가상의 답변을 생성하고 Gemini Embedding 2가 이를 임베딩해 평균을 구한 뒤, 그 결과로 ChromaDB에서 더 정확한 청크를 검색합니다.
- [**록 음악 RAG**](./rag_apps/rock_music_rag) — Wikipedia를 바탕으로 구축하는 맞춤형 록 음악 지식 베이스입니다. 밴드를 추가하고 여러 밴드에 걸쳐 질문하면 BM25 검색과 Gemma 4가 출처를 포함한 답변을 제공합니다.
- [**데이터베이스 라우팅 RAG 에이전트**](./rag_apps/rag_agent_with_database_routing) — Agno 라우터 에이전트로 질의를 제품, 지원, 재무용 Qdrant 데이터베이스 세 곳에 분배합니다. 관련 문서를 찾지 못하면 LangGraph ReAct 웹 검색 에이전트를 사용합니다.
- [**추론 RAG**](./rag_apps/reasoning_rag) — 웹 자료에 대해 질문하면 Gradio를 통해 단계별 추론 과정을 실시간으로 확인하며 출처가 포함된 답변을 받을 수 있습니다.

### 🎛️ 파인튜닝

특화된 작업에 맞춰 모델을 학습하고 파인튜닝하는 프로젝트입니다.

- [**텍스트-SQL 재고 관리 전문가**](./fine_tuning/text_to_sql_inventory) — 파인튜닝한 Qwen3.5-2B 모델을 사용하는 소매 재고 데이터베이스용 자연어 인터페이스입니다. 일상적인 영어로 질문하면 Gradio에서 SQL에 기반한 답변을 받을 수 있습니다.

---

## 🤝 기여하기

기여를 환영합니다! 새 프로젝트 추가, 기존 프로젝트 개선, 버그 수정 등 여러분의 참여가 이 저장소를 모두에게 더 유용한 공간으로 만듭니다.

### 기여 방법

1. **가이드라인 읽기**: 자세한 지침은 [CONTRIBUTING.md](CONTRIBUTING.md)를 확인하세요.
2. **이슈 생성**: 프로젝트나 개선 사항을 제안하세요.
3. **구조 준수**: 알맞은 분류 폴더를 사용하세요.
4. **PR 제출**: 풀 리퀘스트 하나당 프로젝트 하나를 제출하세요.

### 프로젝트 구조 요구사항

- 각 프로젝트는 알맞은 분류 아래의 개별 폴더에 있어야 합니다.
- 상세한 `README.md`를 포함해야 합니다([템플릿](.github/README_TEMPLATE.md) 사용).
- `requirements.txt` 또는 `pyproject.toml`을 포함해야 합니다.
- 필요한 API 키를 안내하는 `.env.example`을 포함해야 합니다.
- snake_case 명명 규칙을 따르세요.

---

## 📜 라이선스

이 저장소는 **MIT 라이선스**로 배포됩니다. 자세한 내용은 [LICENSE](./LICENSE) 파일을 확인하세요.

---

## 🙏 감사의 말

이 AI 엔지니어링 프로젝트 모음을 만드는 데 도움을 주신 모든 기여자 여러분께 감사드립니다!

---

<div align="center">

**[AI Engineering 커뮤니티](https://aiengineering.beehiiv.com/)가 ❤️를 담아 만들었습니다.**

후원이나 협업 문의는 관리자 이메일 [sumanth@devable.ai](mailto:sumanth@devable.ai)로 보내주세요.

[⬆ 맨 위로](#-hands-on-ai-engineering)

</div>
