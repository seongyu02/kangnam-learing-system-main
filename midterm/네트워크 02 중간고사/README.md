# 네트워크 02 중간고사

## 중간고사 범위

**네트워크 서비스 로드맵과 DB 설계 로드맵의 Phase 1~5 전체(Phase 5 포함)**가 범위다. 아래는 우선 학습할 핵심 자료·확인 항목 **46개**를 고른 체크리스트다. 전체 범위는 각 Phase의 원문에서 확인한다. 강의 파일은 이 체크리스트와 공통 체크리스트에 있는 것만 저장소에 남아 있다.

두 팀 공통 범위인 **3~6주차 수업 내용**([공통 체크리스트](../%EA%B3%B5%ED%86%B5%203~6%EC%A3%BC%EC%B0%A8%20%EC%88%98%EC%97%85/README.md))도 함께 본다.

자료를 읽고 옆에 적힌 핵심을 설명하거나 실습할 수 있으면 `[x]`로 표시한다.

## 네트워크 서비스 로드맵

[로드맵 전체 보기](../../study-progress/%EB%84%A4%ED%8A%B8%EC%9B%8C%ED%81%AC%20%EC%84%9C%EB%B9%84%EC%8A%A4%20%EB%A1%9C%EB%93%9C%EB%A7%B5/README.md)

### 01 Phase 1 - 패킷이 어떻게 오가는가

[Phase 전체 자료 보기](../../study-progress/%EB%84%A4%ED%8A%B8%EC%9B%8C%ED%81%AC%20%EC%84%9C%EB%B9%84%EC%8A%A4%20%EB%A1%9C%EB%93%9C%EB%A7%B5/01%20Phase%201%20-%20%ED%8C%A8%ED%82%B7%EC%9D%B4%20%EC%96%B4%EB%96%BB%EA%B2%8C%20%EC%98%A4%EA%B0%80%EB%8A%94%EA%B0%80.md)

- [ ] [06 The OSI Model](../../courses/DevOps%20and%20SRE/IBM%20DevOps%20and%20Software/13%20Application%20Security/Module%201%20-%20Introduction/06%20The%20OSI%20Model.md) — OSI 계층별 역할을 구분한다
- [ ] [01 Lecture 1 - Encapsulation](../../courses/Others/Hands-on%20Internet%20of%20Things/Course%203%20-%20IoT%20Networking/Module%203%20-%20Core%20Networking%20Part%201/01%20Lecture%201%20-%20Encapsulation.md) — 데이터가 계층별 헤더로 감싸지는 캡슐화를 설명한다
- [ ] [07 Lecture 6 - Addressing Layers](../../courses/Others/Hands-on%20Internet%20of%20Things/Course%201%20-%20IoT%20Devices/Module%201%20-%20Orientation%20Basics%20and%20Lab/07%20Lecture%206%20-%20Addressing%20Layers.md) — MAC·IP·포트가 맡는 주소 역할을 구분한다
- [ ] [01 Lecture 8 - Address Resolution Protocol](../../courses/Others/Hands-on%20Internet%20of%20Things/Course%203%20-%20IoT%20Networking/Module%204%20-%20Core%20Networking%20Part%202/01%20Lecture%208%20-%20Address%20Resolution%20Protocol.md) — IP 주소로 MAC 주소를 찾는 ARP 과정을 설명한다
- [ ] [04 Lecture 11 - Sockets API Programming](../../courses/Others/Hands-on%20Internet%20of%20Things/Course%203%20-%20IoT%20Networking/Module%204%20-%20Core%20Networking%20Part%202/04%20Lecture%2011%20-%20Sockets%20API%20Programming.md) — 서버의 bind·listen·accept와 소켓의 역할을 이해한다
- [ ] [11 CIDR](../../courses/Computer%20Science/The%20Bits%20and%20Bytes%20of%20Computer/Module%202%20-%20The%20Network%20Layer/11%20CIDR.md) — CIDR 표기로 네트워크 범위와 호스트 수를 계산한다
- [ ] [12 NAT and the Transport Layer](../../courses/Computer%20Science/The%20Bits%20and%20Bytes%20of%20Computer/Module%204%20-%20Networking%20Services/12%20NAT%20and%20the%20Transport%20Layer.md) — NAT의 포트 변환과 포트 포워딩을 설명한다

### 02 Phase 2 - 이름 붙이기 DNS

[Phase 전체 자료 보기](../../study-progress/%EB%84%A4%ED%8A%B8%EC%9B%8C%ED%81%AC%20%EC%84%9C%EB%B9%84%EC%8A%A4%20%EB%A1%9C%EB%93%9C%EB%A7%B5/02%20Phase%202%20-%20%EC%9D%B4%EB%A6%84%20%EB%B6%99%EC%9D%B4%EA%B8%B0%20DNS.md)

- [ ] [03 The Many Steps of Name Resolution](../../courses/Computer%20Science/The%20Bits%20and%20Bytes%20of%20Computer/Module%204%20-%20Networking%20Services/03%20The%20Many%20Steps%20of%20Name%20Resolution.md) — 재귀 조회·루트·TLD·권한 서버와 TTL·캐시 흐름을 설명한다
- [ ] [06 Resource Record Types](../../courses/Computer%20Science/The%20Bits%20and%20Bytes%20of%20Computer/Module%204%20-%20Networking%20Services/06%20Resource%20Record%20Types.md) — A·AAAA·CNAME·MX·TXT 등 주요 레코드의 용도를 구분한다
- [ ] [08 DNS Zones](../../courses/Computer%20Science/The%20Bits%20and%20Bytes%20of%20Computer/Module%204%20-%20Networking%20Services/08%20DNS%20Zones.md) — DNS 존과 SOA·NS 레코드의 역할을 이해한다
- [ ] [05 Name Resolution Tools](../../courses/Computer%20Science/The%20Bits%20and%20Bytes%20of%20Computer/Module%206%20-%20Troubleshooting/05%20Name%20Resolution%20Tools.md) — 조회 대상 서버와 레코드 유형을 바꿔 DNS 응답을 진단한다

### 03 Phase 3 - HTTP와 API

[Phase 전체 자료 보기](../../study-progress/%EB%84%A4%ED%8A%B8%EC%9B%8C%ED%81%AC%20%EC%84%9C%EB%B9%84%EC%8A%A4%20%EB%A1%9C%EB%93%9C%EB%A7%B5/03%20Phase%203%20-%20HTTP%EC%99%80%20API.md)

- [ ] [06 4.1.6 – HTTP](../../courses/Computer%20Science/Software%20Design/Course%204%20-%20Service-Oriented/Module%201%20-%20Web%20Technologies/06%204.1.6%20%E2%80%93%20HTTP.md) — HTTP 메서드·상태 코드·헤더를 읽는다
- [ ] [02 4.3.2 – Designing a REST Service](../../courses/Computer%20Science/Software%20Design/Course%204%20-%20Service-Oriented/Module%203%20-%20REST%20Architecture/02%204.3.2%20%E2%80%93%20Designing%20a%20REST%20Service.md) — 자원과 메서드 중심으로 REST API를 설계한다
- [ ] [04 Making API Requests using CURL and Postman](../../courses/DevOps%20and%20SRE/IBM%20DevOps%20and%20Software/10%20Microservices%20and%20Serverless/Module%202%20-%20Web%20API%20Essentials/04%20Making%20API%20Requests%20using%20CURL.md) — curl로 요청을 보내 응답과 오류를 확인한다
- [ ] [05 Reminder on Cookies vs JWT's](../../courses/Microservices%20with%20Node%20JS%20and%20React/Section%209%20-%20Authentication%20Strategies%20and%20Options/05%20Reminder%20on%20Cookies%20vs%20JWT's.md) — 쿠키·서버 세션·JWT의 차이를 설명한다
- [ ] [12 Handling CORS Errors](../../courses/Microservices%20with%20Node%20JS%20and%20React/Section%202%20-%20A%20Mini-Microservices%20App/12%20Handling%20CORS%20Errors.md) — CORS 오류가 발생하는 조건과 해결 흐름을 이해한다

### 04 Phase 4 - 암호화와 신뢰 TLS

[Phase 전체 자료 보기](../../study-progress/%EB%84%A4%ED%8A%B8%EC%9B%8C%ED%81%AC%20%EC%84%9C%EB%B9%84%EC%8A%A4%20%EB%A1%9C%EB%93%9C%EB%A7%B5/04%20Phase%204%20-%20%EC%95%94%ED%98%B8%ED%99%94%EC%99%80%20%EC%8B%A0%EB%A2%B0%20TLS.md)

- [ ] [09 TLS-SSL](../../courses/DevOps%20and%20SRE/IBM%20DevOps%20and%20Software/13%20Application%20Security/Module%201%20-%20Introduction/09%20TLS-SSL.md) — TLS 핸드셰이크와 서버 신원 검증·세션 키의 역할을 설명한다
- [ ] [10 What Is OpenSSL](../../courses/DevOps%20and%20SRE/IBM%20DevOps%20and%20Software/13%20Application%20Security/Module%201%20-%20Introduction/10%20What%20Is%20OpenSSL.md) — OpenSSL을 인증서와 TLS 연결 진단에 사용한다
- [ ] [03.Demonstration - Implementing HTTPS for an API](../../courses/Web%20and%20APIs/Protecting%20and%20Managing%20APIs/Module%201%20-%20API%20Security/Lesson%204%20-%20Encryption/03.Demonstration%20-%20Implementing%20HTTPS%20for%20an%20API.md) — API에 HTTPS를 적용하는 과정을 확인한다
- [ ] [인증서 체인·CA·신뢰 확인](../../study-progress/%EB%84%A4%ED%8A%B8%EC%9B%8C%ED%81%AC%20%EC%84%9C%EB%B9%84%EC%8A%A4%20%EB%A1%9C%EB%93%9C%EB%A7%B5/04%20Phase%204%20-%20%EC%95%94%ED%98%B8%ED%99%94%EC%99%80%20%EC%8B%A0%EB%A2%B0%20TLS.md) — 4-C와 산출물 과제에서 인증서 발급자·유효기간·신뢰 체인을 확인한다

### 05 Phase 5 - 프록시와 로드밸런싱

[Phase 전체 자료 보기](../../study-progress/%EB%84%A4%ED%8A%B8%EC%9B%8C%ED%81%AC%20%EC%84%9C%EB%B9%84%EC%8A%A4%20%EB%A1%9C%EB%93%9C%EB%A7%B5/05%20Phase%205%20-%20%ED%94%84%EB%A1%9D%EC%8B%9C%EC%99%80%20%EB%A1%9C%EB%93%9C%EB%B0%B8%EB%9F%B0%EC%8B%B1.md)

- [ ] [03.Routing and Proxying](../../courses/Web%20and%20APIs/Protecting%20and%20Managing%20APIs/Module%202%20-%20API%20Management/Lesson%201%20-%20API%20Gateways/03.Routing%20and%20Proxying.md) — 프록시가 요청을 받아 백엔드로 전달하는 흐름을 설명한다
- [ ] [02 Network - Load Balancer](../../courses/NAVER%20Cloud%20Platform%20Boot%20Camp%20-%20%EB%84%A4%EC%9D%B4%EB%B2%84%20%ED%81%B4%EB%9D%BC%EC%9A%B0%EB%93%9C%20%EB%B6%80%ED%8A%B8%20%EC%BA%A0%ED%94%84/Section%204%20-%20Network/02%20Network%20-%20Load%20Balancer.md) — L4·L7 로드밸런서와 분산 알고리즘의 차이를 구분한다
- [ ] [04 Network - Application Load Balancer](../../courses/NAVER%20Cloud%20Platform%20Boot%20Camp%20-%20%EB%84%A4%EC%9D%B4%EB%B2%84%20%ED%81%B4%EB%9D%BC%EC%9A%B0%EB%93%9C%20%EB%B6%80%ED%8A%B8%20%EC%BA%A0%ED%94%84/Section%204%20-%20Network/04%20Network%20-%20Application%20Load%20Balancer.md) — 대상 그룹과 헬스체크를 설정해 정상 서버로 요청을 보낸다
- [ ] [06 Network - Network Proxy Load Balancer](../../courses/NAVER%20Cloud%20Platform%20Boot%20Camp%20-%20%EB%84%A4%EC%9D%B4%EB%B2%84%20%ED%81%B4%EB%9D%BC%EC%9A%B0%EB%93%9C%20%EB%B6%80%ED%8A%B8%20%EC%BA%A0%ED%94%84/Section%204%20-%20Network/06%20Network%20-%20Network%20Proxy%20Load%20Balancer.md) — 프록시 로드밸런서의 TLS 종료 위치를 설명한다
- [ ] [13 CDN - Content Delivery Networks](../../courses/DevOps%20and%20SRE/IBM%20DevOps%20and%20Software/02%20Introduction%20to%20Cloud/Module%203%20-%20Components%20of%20Cloud/13%20CDN%20-%20Content%20Delivery%20Networks.md) — CDN·캐시가 요청 경로에 놓이는 위치와 역할을 이해한다

## DB 설계 로드맵

[로드맵 전체 보기](../../study-progress/DB%20%EC%84%A4%EA%B3%84%20%EB%A1%9C%EB%93%9C%EB%A7%B5/README.md)

### 01 Phase 1 - 설계 프로세스와 요구사항 수집

[Phase 전체 자료 보기](../../study-progress/DB%20%EC%84%A4%EA%B3%84%20%EB%A1%9C%EB%93%9C%EB%A7%B5/01%20Phase%201%20-%20%EC%84%A4%EA%B3%84%20%ED%94%84%EB%A1%9C%EC%84%B8%EC%8A%A4%EC%99%80%20%EC%9A%94%EA%B5%AC%EC%82%AC%ED%95%AD%20%EC%88%98%EC%A7%91.md)

- [ ] [03 Identify Database Components](../../courses/Databases%20and%20SQL/Database%20Design%20-%20A%20Modern%20Approach/Module%201%20-%20Getting%20Started%20with%20Relational/03%20Identify%20Database%20Components.md) — 테이블·행·열·키의 역할을 구분한다
- [ ] [04 Identify Common Database Design Problems](../../courses/Databases%20and%20SQL/Database%20Design%20-%20A%20Modern%20Approach/Module%201%20-%20Getting%20Started%20with%20Relational/04%20Identify%20Common%20Database%20Design%20Problems.md) — 갱신·삽입·삭제 이상을 구분한다
- [ ] [05 Follow a Database Design Process](../../courses/Databases%20and%20SQL/Database%20Design%20-%20A%20Modern%20Approach/Module%201%20-%20Getting%20Started%20with%20Relational/05%20Follow%20a%20Database%20Design%20Process.md) — 개념·논리·물리 설계 단계의 역할을 구분한다
- [ ] [06 Gather Requirements](../../courses/Databases%20and%20SQL/Database%20Design%20-%20A%20Modern%20Approach/Module%201%20-%20Getting%20Started%20with%20Relational/06%20Gather%20Requirements.md) — 요구사항에서 데이터와 업무 규칙을 추출한다

### 02 Phase 2 - 개념 모델과 ERD

[Phase 전체 자료 보기](../../study-progress/DB%20%EC%84%A4%EA%B3%84%20%EB%A1%9C%EB%93%9C%EB%A7%B5/02%20Phase%202%20-%20%EA%B0%9C%EB%85%90%20%EB%AA%A8%EB%8D%B8%EA%B3%BC%20ERD.md)

- [ ] [05 What are Entities and Attributes (Identifiers)](../../courses/Databases%20and%20SQL/Relational%20Database%20Design/Module%201%20-%20Introduction%20to%20DBMS%20and%20Entity/05%20What%20are%20Entities%20and%20Attributes%20(Identifiers).md) — 엔티티와 속성을 구분한다
- [ ] [06 What are Relationships - Degree, Cardinality and Participation](../../courses/Databases%20and%20SQL/Relational%20Database%20Design/Module%201%20-%20Introduction%20to%20DBMS%20and%20Entity/06%20What%20are%20Relationships%20-%20Degree,%20Cardinality.md) — 관계의 차수·카디널리티·참여 제약을 판정한다
- [ ] [08 Crow's Foot Notation](../../courses/Databases%20and%20SQL/Relational%20Database%20Design/Module%201%20-%20Introduction%20to%20DBMS%20and%20Entity/08%20Crow's%20Foot%20Notation.md) — 까마귀발 표기법으로 관계를 읽는다
- [ ] [09 In-Class Exercise (Drawing an ERD)](../../courses/Databases%20and%20SQL/Relational%20Database%20Design/Module%201%20-%20Introduction%20to%20DBMS%20and%20Entity/09%20In-Class%20Exercise%20(Drawing%20an%20ERD).md) — 요구사항을 바탕으로 ERD를 직접 그린다

### 03 Phase 3 - 논리 모델과 키

[Phase 전체 자료 보기](../../study-progress/DB%20%EC%84%A4%EA%B3%84%20%EB%A1%9C%EB%93%9C%EB%A7%B5/03%20Phase%203%20-%20%EB%85%BC%EB%A6%AC%20%EB%AA%A8%EB%8D%B8%EA%B3%BC%20%ED%82%A4.md)

- [ ] [02 What are Keys](../../courses/Databases%20and%20SQL/Relational%20Database%20Design/Module%202%20-%20Relational%20Models/02%20What%20are%20Keys.md) — 후보키·기본키·대체키·복합키를 구분한다
- [ ] [03 Keys](../../courses/Databases%20and%20SQL/PostgreSQL%20for%20Everybody/Course%201%20-%20Database%20Design/Module%203%20-%20One-To-Many%20Data%20Models/03%20Keys.md) — 자연키와 대리키의 선택 근거를 설명한다
- [ ] [06 Foreign key](../../courses/Databases%20and%20SQL/Meta%20Database%20Engineer/01%20Introduction%20to%20Databases/Module%204%20-%20Database%20design/06%20Foreign%20key.md) — 외래키와 참조 무결성의 역할을 이해한다
- [ ] [04 How to Convert ERDs to Relational Models](../../courses/Databases%20and%20SQL/Relational%20Database%20Design/Module%202%20-%20Relational%20Models/04%20How%20to%20Convert%20ERDs%20to%20Relational%20Models.md) — ERD의 관계를 테이블과 키로 변환한다

### 04 Phase 4 - 정규화와 함수 종속

[Phase 전체 자료 보기](../../study-progress/DB%20%EC%84%A4%EA%B3%84%20%EB%A1%9C%EB%93%9C%EB%A7%B5/04%20Phase%204%20-%20%EC%A0%95%EA%B7%9C%ED%99%94%EC%99%80%20%ED%95%A8%EC%88%98%20%EC%A2%85%EC%86%8D.md)

- [ ] [01 Functional Dependency (FD)](../../courses/Databases%20and%20SQL/Relational%20Database%20Design%20(Illinois%20Tech)/Module%202%20-%20Functional%20Dependency/01%20Functional%20Dependency%20(FD).md) — 업무 규칙에서 함수 종속 X → Y를 찾는다
- [ ] [02 Attribute Closure and Candidate Keys](../../courses/Databases%20and%20SQL/Relational%20Database%20Design%20(Illinois%20Tech)/Module%202%20-%20Functional%20Dependency/02%20Attribute%20Closure%20and%20Candidate%20Keys.md) — 속성 폐포로 후보키를 구한다
- [ ] [03 Full Partial and Transitive Functional Dependencies](../../courses/Databases%20and%20SQL/Relational%20Database%20Design/Module%203%20-%20Normalization/03%20Full%20Partial%20and%20Transitive%20Functional%20Dependencies.md) — 완전·부분·이행 종속을 구분한다
- [ ] [04 Normal Forms and Normalization Process](../../courses/Databases%20and%20SQL/Relational%20Database%20Design/Module%203%20-%20Normalization/04%20Normal%20Forms%20and%20Normalization%20Process.md) — 1NF·2NF·3NF를 판정하고 테이블을 분해한다
- [ ] [02 Boyce-Codd Normal Form](../../courses/Databases%20and%20SQL/Relational%20Database%20Design%20(Illinois%20Tech)/Module%203%20-%20Database%20Normalization/02%20Boyce-Codd%20Normal%20Form.md) — BCNF와 3NF의 차이를 설명한다

### 05 Phase 5 - 다대다와 이력 설계

[Phase 전체 자료 보기](../../study-progress/DB%20%EC%84%A4%EA%B3%84%20%EB%A1%9C%EB%93%9C%EB%A7%B5/05%20Phase%205%20-%20%EB%8B%A4%EB%8C%80%EB%8B%A4%EC%99%80%20%EC%9D%B4%EB%A0%A5%20%EC%84%A4%EA%B3%84.md)

- [ ] [01 Many-to-Many Relationships](../../courses/Databases%20and%20SQL/PostgreSQL%20for%20Everybody/Course%201%20-%20Database%20Design/Module%204%20-%20Many-To-Many%20Data/01%20Many-to-Many%20Relationships.md) — N:M 관계를 연결 테이블로 풀고 기본키를 정한다
- [ ] [02 Demonstration - Database Design and Many to Many](../../courses/Databases%20and%20SQL/PostgreSQL%20for%20Everybody/Course%201%20-%20Database%20Design/Module%204%20-%20Many-To-Many%20Data/02%20Demonstration%20-%20Database%20Design%20and%20Many.md) — 다대다 관계를 실제 테이블로 구현한다
- [ ] [02 Understanding SCD2 Core Components and Business Logic](../../courses/Data%20Engineering/Open%20Source%20Data%20Engineering/Course%201%20-%20Building%20Automated/Module%207%20-%20SCD2%20Historical/02%20Understanding%20SCD2%20Core%20Components.md) — 이력의 유효 시작·종료 시각과 현재 상태를 구분한다
- [ ] [03 Building Your First SCD2 Table Structure in SQL](../../courses/Data%20Engineering/Open%20Source%20Data%20Engineering/Course%201%20-%20Building%20Automated/Module%207%20-%20SCD2%20Historical/03%20Building%20Your%20First%20SCD2%20Table.md) — SCD2 테이블을 SQL로 만들고 과거 상태를 보존한다

**함께 확인할 핵심:** 관계 자체의 속성은 연결 테이블에 두고, 로드맵 구성과 학습 사건을 같은 행으로 표현할지 분리할지 판단한다. [Phase 5의 5-B 절](../../study-progress/DB%20%EC%84%A4%EA%B3%84%20%EB%A1%9C%EB%93%9C%EB%A7%B5/05%20Phase%205%20-%20%EB%8B%A4%EB%8C%80%EB%8B%A4%EC%99%80%20%EC%9D%B4%EB%A0%A5%20%EC%84%A4%EA%B3%84.md)을 확인한다.

[중간고사 안내로 돌아가기](../README.md)
