# Phase 4 — 회사 지식과 시스템 연결

- 목표: 에이전트가 회사의 문서·대화·데이터·시스템을 스스로 조회할 수 있는 상태 — 빌더 조쉬 사례가 말하는 **"조회 가능한 환경(queryable environment)"** — 을 만든다.
- 분량: 약 14시간
- 마지막 학습일: (미학습)

## 이 단계가 끝나면 할 수 있어야 하는 것

- 사내 문서와 대화를 검색 가능한 지식베이스로 만들고, 검색이 잘 되는지 숫자로 확인할 수 있다.
- 흩어진 암묵지를 에이전트가 반복해서 쓸 수 있는 **스킬** 형태로 옮길 수 있다.
- 사내 시스템(DB·이슈 트래커·메신저·메일)을 MCP 서버로 감싸 에이전트에 붙일 수 있다.
- 어떤 사내 데이터를 외부 모델에 넣어도 되는지 기준을 세우고 그 근거를 말할 수 있다.

> **이 Phase부터 실제 사내 데이터를 다룬다.** 4-D를 먼저 읽고 투입 기준을 정한 뒤 4-B의 색인 작업을 시작하는 편이 안전하다.

## 4-A. 암묵지를 문서로 옮기고 스킬로 굳힌다

메인: AI Agent Skills for Leaders 전체. **일회성 프롬프트를 회사의 자산으로 바꾸는 방법**이 이 강좌의 전부다. 25강이지만 강의가 짧다.

- [ ] 01 Seeing Skills in Action.md
- [ ] 02 Skills are On-demand Training for AI Agents.md — **스킬 = 에이전트에게 필요할 때 주는 훈련.** 신입 교육 자료를 에이전트용으로 바꾼다는 관점이 여기서 나온다.
- [ ] 03 Creating a Skill Manually.md
- [ ] 04 Building a Dashboarding Skill.md — Phase 9의 계기판과 직접 연결된다.
- [ ] 06 Creating a Skill in Chat with a Skill Creator.md
- [ ] 02 Using AI Memory to Build Skills.md
- [ ] 03 Turn a Conversation into Skill.md — **대화를 스킬로 승격.** 사내 암묵지를 뽑아내는 가장 현실적인 경로다.
- [ ] 01 The Anatomy of a Skill.md
- [ ] 02 The Skill.md File - Instructions and Context for Your AI Agent.md
- [ ] 03 Scripts - Tools for Your AI Agent.md
- [ ] 05 Assets - Data, Templates, and More for the AI Agent to Work With.md — 사내 양식·템플릿을 여기에 넣는다.
- [ ] 06 References - Contextual Depth, Patterns, Examples for the AI Agent.md
- [ ] [01 The RECIPE Framework.md](../../courses/AI%20Agents%20and%20Generative%20AI/AI%20Agent%20Skills%20for%20Leaders/Module%204%20-%20The%20RECIPE%20for%20Skills/01%20The%20RECIPE%20Framework.md) — **RECIPE 프레임워크.** 이 Phase 산출물의 작성 형식.
- [ ] 02 Requests.md
- [ ] 03 Environment.md
- [ ] 04 Concrete Steps.md
- [ ] 05 Ideal Result.md
- [ ] 09 Refining a Skill.md
- [ ] 10 Contextual Preferences Pattern.md — 회사 고유의 선호(톤·양식·금지 표현)를 스킬에 심는 패턴.

함께 보기: 실무자 관점의 짧은 자료들.

- [ ] 2026-07-04 좋은 Agent Skill을 만드는 방법.md
- [ ] 2026-06-29 Building Great Agent Skills - The Missing Manual.md
- [ ] 15 Day 4 - Deep Agents Skills Explained - SKILL.md and Progressive Disclosure.md — **점진적 공개(progressive disclosure).** 스킬이 많아졌을 때 컨텍스트가 터지지 않게 하는 방법.
- [ ] 03 CLAUDE.md and Project Context.md — 프로젝트 상시 맥락 파일. 회사 단위로 확장하면 "회사 헌법"이 된다(Phase 5).
- [ ] 04 Coding Standards and AI Interaction Rules.md

## 4-B. 지식베이스(RAG)를 만든다

메인: Retrieval Augmented Generation. **module 02가 이 Phase의 핵심**이다 — 검색이 나쁘면 그 뒤가 전부 무의미하다.

module 01 — 기본기

- [ ] 03 Introduction to RAG.md
- [ ] [05 RAG Architecture Overview.md](../../courses/Retrieval%20Augmented%20Generation/module%2001/05%20RAG%20Architecture%20Overview.md)
- [ ] 07 Introduction to Information Retrieval.md

module 02 — 검색기

- [ ] 02 Retriever Architecture Overview.md
- [ ] 03 Metadata Filtering.md — **메타데이터 필터링.** 사내 문서는 부서·기간·비밀등급으로 걸러야 해서 이게 특히 중요하다.
- [ ] 05 Keyword Search - BM25.md
- [ ] 06 Semantic Search - Introduction.md
- [ ] 07 Semantic Search - Embedding Model Deepdive.md
- [ ] 08 Hybrid Search.md — **하이브리드 검색.** 사내 용어·제품명이 많은 회사 문서에서 키워드와 의미 검색을 섞는 이유.
- [ ] 09 Evaluating Retrieval.md — **검색 품질 평가.** 이걸 안 하면 "왜 답이 이상한지"를 영원히 모른다.

module 03 — 저장과 전처리

- [ ] 03 Vector Databases.md
- [ ] [04 Chunking.md](../../courses/Retrieval%20Augmented%20Generation/module%2003/04%20Chunking.md) — **청킹.** 회의록·위키·Slack 로그는 형태가 제각각이라 여기서 대부분의 품질이 갈린다.
- [ ] 05 Advanced Chunking Techniques.md
- [ ] 06 Query Parsing.md
- [ ] 08 Reranking.md

module 05 — 운영

- [ ] 02 What Makes Production Challenging.md — **문서가 계속 바뀌는 회사 환경에서 무엇이 깨지는가.** 재색인 주기를 정하는 근거.
- [ ] 03 Implementing RAG Evaluation Strategies.md

함께 보기:

- [ ] 09 Agentic RAG.md — 에이전트가 검색 자체를 판단하며 반복하는 구조.
- [ ] 03 Agentic RAG - Enhance Retrieval with Multi-Agent Systems.md
- [ ] 15 Day 3 - Agentic RAG with the Qdrant MCP Server for AI Agents.md — RAG를 MCP 서버로 노출하는 실습. 4-C와 이어서 본다.

## 4-C. 사내 시스템을 MCP로 연결한다

> ### 사내 MCP 서버를 만들 때 지켜야 하는 것
>
> 아래 강의는 **개념**을 위해 본다 — 호스트·클라이언트·서버 분리, 도구 명세를 어떻게 쓰는가, 왜 기존 사내 API를 그대로 붙이면 안 되는가. **프로토콜 세부는 강의가 아니라 [공식 스펙](https://modelcontextprotocol.io/specification/2026-07-28)에서 가져온다.** 실제로 서버를 만들 때 지켜야 하는 것은 아래와 같다.
>
> - **상태를 두지 않는다.** 세션도 연결 시 핸드셰이크도 없다. 요청마다 `_meta`에 프로토콜 버전과 클라이언트 능력이 실려 온다. 호출 사이에 상태가 필요하면 **서버가 발급한 handle을 평범한 툴 인자로** 주고받는다.
> - **`server/discover` RPC를 구현한다.** 필수다. 지원 버전·능력·신원을 여기서 광고한다.
> - **LLM이 필요하면 제공자 API를 직접 호출한다.** 서버가 클라이언트의 모델을 빌려 쓰는 경로는 없다.
> - **파일 경로나 작업 범위는 툴 인자·리소스 URI·서버 설정으로 받는다.**
> - **사람 확인이 필요하면 MRTR을 쓴다** — `resultType: "input_required"` 와 `inputRequests` 를 돌려주고, 클라이언트가 `inputResponses` 를 실어 원 요청을 다시 보낸다. **서버는 승인을 기다리며 붙잡고 있지 않는다.** 승인 대기를 이어 붙이려면 서버가 발급한 식별자를 `requestState`에 담는다. → [Phase 5의 승인 지점](05%20Phase%205%20-%20에이전트%20조직%20만들기.md)
> - **로그는 stdio면 stderr, 그 밖에는 OpenTelemetry로 낸다.** `_meta`의 `traceparent`/`tracestate`로 트레이스 컨텍스트를 전파한다. → Phase 7
> - **전송은 Streamable HTTP.** 스트림이 끊기면 새 요청 ID로 재발행한다 — 끊긴 자리에서 재개하는 경로는 없다.
> - **목록 결과에 `ttlMs`/`cacheScope`를 실어** 클라이언트가 캐시하게 한다. 사내 도구가 10개를 넘어가면 폴링 비용이 여기서 갈린다.
> - **인가는 Client ID Metadata Documents로.** 인가 응답의 `iss`를 반드시 검증한다.
>
> 도구 목록은 **매번 같은 순서로** 돌려준다. 클라이언트 캐시와 프롬프트 캐시 적중률이 여기 달려 있다.


메인: AI Agents with Model Context Protocol (13강 전체). 개념이 가장 정돈돼 있다.

- [ ] 01 Why Do We Need Model Context Protocol.md
- [ ] 02 Model Context Protocol and AI Problem Solving with Tools.md
- [ ] 03 MCP Allows AI to Communicate with the Computer.md
- [ ] 01 Model Context Protocol - Syntax, Semantics, Timing.md
- [ ] [03 What is an MCP Server.md](../../courses/AI%20Agents%20and%20Generative%20AI/AI%20Agents%20with%20Model%20Context%20Protocol/Module%202%20-%20AI%20Agent%20Loops%20and%20Model/03%20What%20is%20an%20MCP%20Server.md)
- [ ] 04 Tool Specifications.md
- [ ] 05 Agents Talking to Tools vs. Tools with AI.md
- [ ] 01 Resources.md
- [ ] 01 Prompts and MCP.md

메인 실습: AI Engineer Agentic Track, Week 6. **직접 MCP 서버를 만드는 부분이 이 Phase 산출물의 뼈대다.**

- [ ] **02 Day 1 - What Is MCP Host, Client and Server Architecture Explained.md**
- [ ] 03 Day 1 - How MCP Works - Local vs Remote Servers and Calling Tools.md — 사내 서버를 로컬에 둘지 원격에 둘지 판단 근거.
- [ ] 06 Day 1 - First MCP Lab - Connecting Fetch, Playwright and Filesystem.md
- [ ] 09 Day 2 - Why Build Your Own MCP Server (and When You Shouldn''t).md — **직접 만들지 말아야 할 때.** 사내 시스템마다 서버를 찍어내기 전에 본다.
- [ ] 10 Day 2 - MCP Marketplaces and Building an MCP Server with FastMCP.md — **FastMCP로 직접 서버 만들기.** 산출물의 핵심 실습.
- [ ] 11 Day 2 - Run and Call Your Own MCP Server from an AI Agent.md
- [ ] 12 Day 3 - Context Engineering for AI Agents with MCP Servers.md
- [ ] 13 Day 3 - Long-Term Memory and Web Search MCP Servers for AI Agents.md
- [ ] 16 Day 3 - Market Data MCP Server and Progressive Disclosure of Tools.md — **도구가 많아졌을 때의 점진적 공개.** 사내 시스템을 10개 붙이면 반드시 마주친다.

함께 보기: 개념을 다른 각도에서 한 번 더.

- [ ] 2026-06-24 How Model Context Protocol (MCP) actually works.md
- [ ] **2026-07-01 MCP vs API - Why traditional APIs are failing AI agents.md** — **기존 사내 API를 그대로 붙이면 왜 안 되는가.** 사내 시스템 연결의 판단 근거.
- [ ] 2025-11-17 Building your own MCP server with ADK.md
- [ ] 07 MCP (Model Context Protocol).md
- [ ] 04 MCP As Agent Tool.md

기성 MCP 서버를 붙여 보는 짧은 실습:

- [ ] 11 Introduction to MCP.md
- [ ] 12 Installing the Neon MCP Server.md — **DB를 MCP로 붙이는 실물 예.** 사내 DB 연결의 최소 형태.
- [ ] 14 Installing Playwright MCP.md — 브라우저 자동화. API가 없는 사내 웹 시스템을 붙일 때의 마지막 수단.

## 4-D. 사내 데이터를 넣는 기준

메인: Generative AI and LLM Security, Module 2 앞부분 + MCP 강좌의 보안 강의.

- [ ] 01 The Importance of Secure Data in AI Development.md
- [ ] 03 Best Practices for Securing AI Data Pipelines.md
- [ ] 09 Secure Storage and Key Management for AI Artifacts.md
- [ ] [02 AI Agents, MCP, and Identity - Security.md](../../courses/AI%20Agents%20and%20Generative%20AI/AI%20Agents%20with%20Model%20Context%20Protocol/Module%205%20-%20Faster,%20More/02%20AI%20Agents,%20MCP,%20and%20Identity%20-%20Security.md) — **에이전트에 어떤 신원과 권한을 줄 것인가.** 사내 시스템을 붙이기 전에 반드시 본다.
- [ ] 09 Security.md — 지식베이스 쪽 보안. 문서 접근 권한이 검색 결과에 반영되지 않는 사고가 여기 있다.

전체 위협 지형은 Phase 7에서 다룬다. 여기서는 **"무엇을 넣지 않을 것인가"** 만 정하고 넘어간다.

## 산출물

1. **회사 스킬 세트 3개 이상** — RECIPE 형식으로 작성. 각각 실제 반복 업무 하나를 담당한다. 예: 문의 분류, 주간 보고 초안, 장애 1차 조사.
2. **사내 지식베이스** — Phase 1의 프로세스 지도에 나온 데이터 저장소를 실제로 색인한다. 진실의 원천(source of truth)이 어디인지 목록으로 정리하고, **변하지 않는 문서와 계속 갱신되는 문서를 구분해 후자의 재색인 주기를 정한다.**
3. **검색 품질 리포트** — 실제 사내 질문 20개를 만들어 검색 결과를 채점한다. 정답 문서가 상위 N개에 들어오는 비율을 기록한다. 이 숫자가 없으면 Phase 6의 eval에서 "모델이 틀린 것"과 "검색이 틀린 것"을 구분할 수 없다.
4. **MCP 서버 1개 이상 직접 제작** — 사내 시스템 하나를 감싼다. 도구 이름·설명·권한 범위를 문서화한다.
5. **사내 데이터 투입 기준 문서** — 어떤 데이터가 어느 등급이고 어떤 모델(외부 API / 로컬)까지 갈 수 있는지 표. Phase 7에서 갱신한다.

## 다음 단계

→ [05 Phase 5 - 에이전트 조직 만들기](05%20Phase%205%20-%20에이전트%20조직%20만들기.md)
