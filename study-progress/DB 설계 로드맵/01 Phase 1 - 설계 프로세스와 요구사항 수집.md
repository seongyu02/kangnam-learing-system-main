# Phase 1 — 설계 프로세스와 요구사항 수집

- 목표: 설계가 개념·논리·물리 세 단계로 나뉘는 이유를 알고, learning-hub 저장소의 업무 규칙을 문장으로 뽑아낸다.
- 분량: 약 7시간
- 마지막 학습일: 2026-10-12 (핵심 개념 학습 · Phase 전체 미완료)

## 이 단계가 끝나면 할 수 있어야 하는 것

- 개념 모델·논리 모델·물리 모델이 각각 무엇을 결정하고 무엇을 미루는지 구분해 설명할 수 있다
- 잘못 설계된 테이블이 만드는 갱신·삽입·삭제 이상(anomaly)을 실제 데이터로 재현해 보일 수 있다
- 도메인을 모르는 사람에게서 데이터 요구사항을 끌어내는 질문을 만들 수 있다
- 요구사항 문장에서 엔티티 후보와 관계 후보를 분리해 표로 정리할 수 있다

> **준비물**: MySQL 8 컨테이너 하나. Phase 1에서는 이상(anomaly) 재현에만 쓰지만, 지금 만들어 두면 이후 Phase에서 바로 이어 쓴다. **DB 운영 안정화 로드맵**을 진행 중이라면 그 환경을 그대로 쓴다.

## 1-A. 데이터베이스가 무엇을 해 주는가

메인: Database Design - A Modern Approach, Module 1

- [ ] 01 Getting Started - Course Overview.md — 강좌 전체 지도. 이 로드맵 Phase 1~4·6의 순서가 여기 그대로 있다
- [ ] 02 Lesson Introduction.md
- [ ] [03 Identify Database Components.md](../../courses/Databases%20and%20SQL/Database%20Design%20-%20A%20Modern%20Approach/Module%201%20-%20Getting%20Started%20with%20Relational/03%20Identify%20Database%20Components.md) — 테이블·행·열·키라는 재료 목록

함께 보기: Relational Database Design Module 1 앞부분 — 데이터가 왜 DBMS에 들어가야 하는지를 정보·지식 층위로 설명한다. 더 개론적이다.

- [ ] 01 Course Overview.md
- [ ] 02 Data, Information, Knowledge, and Intelligence.md
- [ ] 03 Solutions for Data Management.md — **파일 저장으로는 왜 안 되는가.** 지금 이 저장소가 Markdown 파일로 진행 기록을 관리하는 방식의 한계와 정확히 겹친다
- [ ] 04 Data Stored in DBMS.md

MySQL 쪽 입문이 필요하면: Meta 01 Introduction to Databases Module 1. 이미 SQL을 쓰고 있다면 건너뛰어도 된다.

- [ ] 04 What is a database.md
- [ ] 05 How is data related.md
- [ ] 11 What are tables in databases.md
- [ ] 12 Types of keys in a database table.md — 키 종류 예고편. 본편은 Phase 3이다

## 1-B. 나쁜 설계가 만드는 문제

**이 절이 Phase 1의 핵심이다.** 정규화를 Phase 4에서 배우게 되는데, 그 전에 "정규화하지 않으면 무슨 일이 벌어지는가"를 몸으로 겪어 둬야 한다. 그러지 않으면 Phase 4가 규칙 암기가 된다.

메인: Database Design - A Modern Approach, Module 1

- [x] [04 Identify Common Database Design Problems.md](../../courses/Databases%20and%20SQL/Database%20Design%20-%20A%20Modern%20Approach/Module%201%20-%20Getting%20Started%20with%20Relational/04%20Identify%20Common%20Database%20Design%20Problems.md) — **갱신·삽입·삭제 이상(update/insert/delete anomaly).** Phase 4 전체가 이 세 가지를 없애는 작업이다 (2026-10-12: 개념 구별 확인, MySQL 재현 실습은 미완료)

함께 보기: 같은 내용을 다른 각도에서

- [ ] 01 Data Redundancy and Normalization.md — 중복이 왜 그 자체로 위험한지
- [ ] 04 Normalization Addresses Anomalies in Database Systems.md — 이상 세 가지를 형식적으로 정리한다

## 1-C. 설계는 3단계로 나뉜다

메인: Database Design - A Modern Approach, Module 1

- [ ] [05 Follow a Database Design Process.md](../../courses/Databases%20and%20SQL/Database%20Design%20-%20A%20Modern%20Approach/Module%201%20-%20Getting%20Started%20with%20Relational/05%20Follow%20a%20Database%20Design%20Process.md) — **개념 → 논리 → 물리.** 이 로드맵 Phase 2·3·6이 각각 여기 대응한다

함께 보기: 3단계 분리의 원조 이론

- [ ] 05 ANSI-SPARC Database Architecture.md — **외부·개념·내부 스키마 3층 구조.** 물리 구현을 바꿔도 응용이 안 깨지는 이유(데이터 독립성)가 여기서 나온다
- [ ] 06 Database Architecture Categories.md — 건너뛰어도 된다. 분산 DB 맥락이라 12 부록에서 다시 만난다

설계를 소프트웨어 설계 일반의 관점에서 보고 싶으면: Software Design and Architecture — 요구사항에서 개념 설계로 가는 같은 구조를 객체지향 쪽에서 설명한다. 체크하지 않는다.

## 1-D. 요구사항을 끌어낸다

메인: Database Design - A Modern Approach, Module 1

- [ ] [06 Gather Requirements.md](../../courses/Databases%20and%20SQL/Database%20Design%20-%20A%20Modern%20Approach/Module%201%20-%20Getting%20Started%20with%20Relational/06%20Gather%20Requirements.md) — **무엇을 묻고 무엇을 문서로 남기는가.** 이 로드맵에서는 내가 나에게 인터뷰하는 셈이지만, 질문 목록을 만들어 두는 훈련 자체가 목적이다
- [ ] 07 Lesson Summary.md

> 요구사항에서 최종 스키마까지 한 번에 훑는 케이스 스터디가 Relational Database Design Module 4에 있다. **지금 보지 않는다** — Phase 9에서 통으로 따라가는 것이 이 로드맵의 마지막 관문이다. 지금 답을 보면 Phase 2~6이 헐거워진다.

## 산출물

이 저장소를 대상으로 아래 세 가지를 만든다. Phase 2의 ERD가 전부 여기서 나온다.

1. **업무 규칙 목록 (30문장 이상)** — "한 코스는 여러 모듈을 가진다", "한 강의는 여러 로드맵 Phase에서 체크될 수 있다", "로드맵은 코스를 소유하거나 참조만 한다", "YouTube 자료에는 모듈 계층이 없다" 처럼 **주어-동사-목적어 문장**으로 적는다. 형용사가 아니라 규칙으로 적는 것이 핵심이다.
   - 재료: **AGENTS.md**의 코스 구조·YouTube 구조·학습 진행 기록 절이 그대로 업무 규칙 문서다. 이미 쓰여 있는 것을 문장 단위로 쪼개면 된다.
2. **현행 구조의 문제점 목록** — 지금 Markdown 체크박스 방식으로는 답하기 어려운 질문을 모은다. 예: "이 강의를 체크한 로드맵이 몇 개인가", "어느 코스가 어느 로드맵에도 안 들어 있는가", "지난달에 몇 강을 봤는가". **이 목록이 Phase 9의 검증 질의 20개가 된다.**
3. **이상(anomaly) 재현 노트** — 일부러 정규화하지 않은 단일 테이블(`강의명, 코스명, 코스카테고리, 로드맵명, 학습일`)을 MySQL에 만들고 샘플 30행을 넣은 뒤, 코스 카테고리를 바꿔 보고(갱신 이상) · 아직 강의가 없는 코스를 넣어 보고(삽입 이상) · 마지막 강의를 지워 보며(삭제 이상) 무슨 일이 벌어지는지 기록한다. **Phase 4에서 이 표로 돌아온다.**

## 다음 단계

→ [02 Phase 2 - 개념 모델과 ERD](02%20Phase%202%20-%20개념%20모델과%20ERD.md)
