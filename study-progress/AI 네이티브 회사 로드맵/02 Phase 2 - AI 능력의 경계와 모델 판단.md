# Phase 2 — AI 능력의 경계와 모델 판단

- 목표: 모델이 무엇을 어떻게 못 하는지 알고, 업무마다 어떤 모델을 얼마만큼의 자율성으로 쓸지 근거를 갖고 정한다.
- 분량: 약 10시간
- 마지막 학습일: (미학습)

## 이 단계가 끝나면 할 수 있어야 하는 것

- LLM이 답을 만드는 과정을 설명하고, 왜 환각이 구조적으로 생기는지 말할 수 있다.
- 업무 하나에 대해 프롬프트 / RAG / 파인튜닝 중 무엇을 쓸지 근거를 대고 고를 수 있다.
- 모델별 토큰 비용을 계산해 한 달 운영비를 추정할 수 있다.
- Phase 1의 자동화 후보마다 자율성 등급(제안만 / 사람 승인 후 실행 / 자동 실행)을 붙일 수 있다.

## 2-A. LLM이 답을 만드는 방식

메인: The Complete Agentic AI Engineering Masterclass 앞부분. 짧고 개념이 선명하다.

- [ ] 01 What is AI Model.md
- [ ] 02 What is Generative AI.md
- [ ] 01 Traditional Engineering vs Generative AI Engineering.md — **결정적(deterministic) 시스템과 확률적 시스템의 차이.** 회사 업무를 여기에 올릴 때 무엇이 달라지는지의 출발점.
- [ ] 01 How LLM Process User Input.md

함께 보기: Retrieval Augmented Generation module 04. 위보다 깊게 들어간다. 왜 같은 질문에 다른 답이 나오는지 알고 싶으면 본다.

- [ ] 02 Transformer Architecture.md
- [ ] 03 LLM Sampling Strategies.md — **샘플링 전략.** 출력의 흔들림을 어디까지 줄일 수 있는지가 여기서 결정된다.

함께 보기: 비개발자에게 설명할 언어가 필요할 때.

- [ ] 02 How Generative AI works.md
- [ ] [08 What LLMs can and cannot do.md](../../courses/Generative%20AI%20for%20Everyone/week%2001%20Introduction%20to%20Generative%20AI/08%20What%20LLMs%20can%20and%20cannot%20do.md)
- [ ] 2026-07-23 AI builder essentials - Tokens, Context Windows, RAG 101.md — 토큰·컨텍스트 윈도우를 한 편으로 정리.

## 2-B. 모델을 고르고 비용을 계산한다

메인: Building Your First Multi-Agent AI System with CrewAI, Module 2 앞부분. **역할마다 다른 모델을 붙이는 관점**이 이 로드맵에 가장 잘 맞는다.

- [ ] 01 LLM Providers and Model Selection.md
- [ ] 02 Configuring Models per Agent Role.md — **역할별 모델 배정.** 판단이 중요한 PM 에이전트와 양이 많은 워커에 같은 모델을 쓸 이유가 없다.
- [ ] [03 Evaluating Cost Latency and Accuracy Trade-offs.md](../../courses/AI%20Agents%20and%20Generative%20AI/Building%20Your%20First%20Multi-Agent%20AI/Module%202%20-%20Prompt%20Context%20and%20Flow/03%20Evaluating%20Cost%20Latency%20and%20Accuracy.md) — **비용·지연·정확도의 3각 트레이드오프.** 모델 선택 기준표의 축이 된다.

함께 보기: 실제 여러 제공자를 붙여 비교해 보는 실습.

- [ ] 14 Day 3 - LLM Providers Compared - OpenAI, Claude, Gemini, Ollama, Groq.md
- [ ] 16 Day 3 - Call 8 LLMs with the OpenAI-Compatible API - GPT, Claude, Gemini.md
- [ ] 17 Day 3 - Install Ollama and Run Local LLMs - Llama, GPT-OSS and Gemma.md — **로컬 모델.** 사내 데이터를 외부에 못 보내는 업무와, 실습 중 API 비용을 줄일 때 쓴다.
- [ ] 18 Day 3 - LLM as a Judge - Rank Multiple LLMs with an Orchestration Flow.md — LLM-as-a-judge. Phase 6의 eval에서 다시 쓴다.

함께 보기: 로컬 배포를 진지하게 볼 때.

- [ ] 01 Local LLM Deployment Strategy 1.md
- [ ] 02 Local LLM Deployment Strategy 2.md

비용 감각:

- [ ] [05 Cost intuition.md](../../courses/Generative%20AI%20for%20Everyone/week%2002%20Generative%20AI%20Projects/05%20Cost%20intuition.md) — **토큰 단가로 운영비를 어림하는 감각.**
- [ ] 09 Choosing a model.md
- [ ] 04 Choosing Your LLM.md

## 2-C. 프롬프트 · RAG · 파인튜닝 중 무엇을 쓸 것인가

메인: Generative AI for Everyone week 02. 이 판단을 가장 짧고 명확하게 다룬다.

- [ ] 06 RAG.md
- [ ] 07 Fine-tuning.md
- [ ] 08 Pretraining.md — 왜 대부분의 회사가 여기까지 갈 필요가 없는지.
- [ ] 10 Instruction tuning and RLHF.md
- [ ] 04 Lifecycle of a generative AI project.md

함께 보기:

- [ ] [10 RAG vs. Fine-Tuning.md](../../courses/Retrieval%20Augmented%20Generation/module%2004/10%20RAG%20vs.%20Fine-Tuning.md) — **판단표 형태로 정리된 버전.** Phase 4에 들어가기 전에 이걸 본다.
- [ ] 01 How RAG Works.md
- [ ] 02 When to use LLM Finetuning.md

## 2-D. 환각과 자율성의 경계

이 절이 이 Phase의 결론이다. **"어디까지 맡길 것인가"** 의 답을 여기서 만든다.

메인: Agentic AI module 01 + RAG module 04.

- [ ] 02 What is Agentic AI.md
- [ ] [03 Autonomy Spectrum.md](../../courses/Agentic%20AI/module%2001/03%20Autonomy%20Spectrum.md) — **자율성 스펙트럼.** 자율성 등급표의 원본. 이 로드맵에서 가장 중요한 개념 강의 중 하나다.
- [ ] 04 Benefits of Agentic Workflows.md
- [ ] 05 Agentic AI Applications.md
- [ ] 07 Handling Hallucinations.md — **환각을 없애는 것이 아니라 다루는 법.**

리스크 쪽:

- [ ] 02 Risks of Agentic AI - What You Need to Know About Autonomous AI.md
- [ ] 12 Day 2 - Agentic AI Risks, Guardrails, Evals and Traps to Avoid.md — **실제로 밟는 함정 목록.** Phase 7에서 다시 쓴다.
- [ ] 04 Hallucination is a New Form of Computing.md — 환각을 결함이 아니라 새로운 계산 방식으로 보는 반대 관점. 앞의 강의들과 나란히 놓고 판단한다.

## 산출물

1. **모델 선택 기준표** — 회사에서 돌릴 업무 유형(판단·요약·분류·생성·코드)별로 어떤 모델을 왜 쓸지, 대안은 무엇인지 표로 적는다. 토큰 단가와 예상 월 호출 수로 운영비 추정치를 함께 넣는다.
2. **업무별 자율성 등급표** — Phase 1의 자동화 후보 우선순위표에 열을 하나 더 붙인다.

   | 자율성 등급 | 뜻 | 조건 |
   |---|---|---|
   | L1 제안 | 에이전트는 초안만 만들고 사람이 전부 검토 | 틀렸을 때 손해가 크거나 외부에 나가는 것 |
   | L2 승인 후 실행 | 에이전트가 실행 계획까지 만들고 사람이 승인 | 되돌릴 수 있고 손해가 제한적인 것 |
   | L3 자동 실행 | 사람 개입 없이 끝까지 | 되돌릴 수 있고 반복적이며 eval로 검증된 것 |

   L3은 Phase 6의 eval을 통과한 뒤에만 부여한다. 이 원칙을 표 위에 명시해 둔다.
3. **"AI에 맡기지 않을 것" 목록** — 등급을 못 매기는 업무. 왜 안 되는지 한 줄씩. Phase 10의 역할 재정의표가 이 목록에서 시작된다.

## 다음 단계

→ [03 Phase 3 - 첫 에이전트 만들기](03%20Phase%203%20-%20첫%20에이전트%20만들기.md)
