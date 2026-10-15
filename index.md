---
layout: cv
title: Joohyung Park's CV
---

# Joohyung Park
Software Engineer

Seoul, KR · [joohyung.park@on-the-ground.org](mailto:joohyung.park@on-the-ground.org) · [Linktree](https://linktr.ee/joohyung.park) · [GitHub](https://github.com/on-the-ground) · [LinkedIn](https://www.linkedin.com/in/joohyung-park-47333ab2/)


## Summary

Backend engineer working on distributed systems and complex domain modeling. 8 years of industry experience at NAVER and Weavrcare, followed by technical book translation and open-source language/runtime work. At NAVER, built and migrated a 100PB+ object storage platform. At Weavrcare (Doctor Palette EMR), redesigned the health insurance billing domain, governed by a 1,000-page guideline revised every 3–6 months.


## Skills

- **Languages:** Go, TypeScript, JavaScript, Kotlin, Java, Python
- **Data / Messaging:** MySQL, PostgreSQL, Redis, MongoDB, Kafka
- **Infra:** Kubernetes, Helm, Consul, Datadog
- **Systems:** Linux kernel I/O stack, eBPF / ftrace / perf tracing
- **Concepts:** DDD, Event-Driven Architecture, Stream Processing


## Experience

### Weavrcare · Backend Developer, Doctor Palette EMR
`Jan 2021 – Jan 2024`

Redesigned the health insurance billing system and optimized its batch pipeline

- Split the 1,000-page billing guideline into bounded contexts and encoded billing rules as TypeScript types using ADTs, isolating the impact of revisions every 3–6 months
- Designed GraphQL schemas as view models, separating domain logic from UI concerns
- Rewrote the in-memory billing batch in a multi-tenant environment as Node.js streams, reducing memory per claim from 100MB to under 5MB and eliminating OOM errors during peak billing periods

### NAVER · Storage Platform Developer, Nubes
`Sep 2016 – Jan 2021`

Built and migrated a 100PB object storage platform

- Migrated 100PB of data and billions of metadata records from legacy distributed storage to Nubes using shadow writes and dual reads, with zero downtime
- Mitigated a cascading gateway failure caused by a company-wide KV cache outage by applying gateway rate limiting and failing read traffic over to a dedicated cluster; then designed a back-pressure architecture to prevent recurrence
- Diagnosed a Consul bottleneck caused by long polling from hundreds of microservice instances and refactored to hierarchical event propagation, resolving orchestrator overload
- Moved VM-based process deployments to microservices on Kubernetes and Helm

### Subsea Cable · DSL and runtime for auditable agent workflows 
`2026 – Present` · [__C Lang](https://4gentsinc.github.io/subsea_cable_webpages/)

Workflow language for agents in high-responsibility domains (finance, large-scale data migration) where traceability and audit are required

- Lazily deduces declarative plans (`.vyg`) into DAGs/streams, allowing reduction rules to change at runtime
- Records lineage between agent intent (Goal) and executed operations (Leaf) as immutable state for audit tracing
- Separates the goal space (ends) from the host (means) and specifies goal arity and cardinality, preventing runaway agent behavior at the system level

### Codeit · Node.js Backend Lead Instructor (Contract)
`Nov 2025 – Dec 2025`

- Lead instructor for a Node.js backend bootcamp for non-CS majors; designed lecture content and led code reviews and assessments

### Ontheground (JPub) · Technical Translator
`Jun 2024 – Nov 2025`

- Translated *Domain Modeling Made Functional* into Korean, rewriting all F# examples in Kotlin and TypeScript
- Negotiated the rewrite with the author, PragProg, and JPub as a condition of the Korean edition
- Extended the Arrow-kt effect handler pattern learned during translation into the open-source Effect-ive Programming libraries

## Personal Projects & Open Source

### Agent Harness Protocol · An Abstraction Port of Agent Harness
`Sep 2026 – Present` · [PyPI](https://pypi.org/project/agent-harness-protocol/)

Business-facing port for delegating work to agent harnesses. Python expression of Kotlin 0.2.3 contract.

- Ported Kotlin AHP 0.2.3 to Python async API (async with, AsyncIterator, frozen dataclasses, Error suffixes)
- Enforced 4 terminal outcomes (Completed/Failed/Cancelled/Unresolved); separated None (unknown/missing) from 0/empty output/usage
- Built 58 conformance scenarios across admission, lifecycle, interaction, cleanup, persistence, bounds, output, accounting; assertions use evidence from execution/storage boundaries, not adapter-reported state
- Published protocol + suites to PyPI with 0 runtime deps; isolated LangGraph adapter as `agent-harness-protocol-langgraph` with explicit support matrix

### Effect-ive Programming
Library that delegates effect and capability handling to dedicated handler actors, for the JVM, JavaScript, and Go

### Event Streaming System
Real-time stream processor prototype in Python and Bytewax

### Strbench
Random load generator and benchmark tool for generic storage backends (Go)

### DDZ on eBPF
User-defined I/O tracing on eBPF (Go / C)


## Talks & Publications

- [*Effect_ive Go*](https://docs.google.com/presentation/d/e/2PACX-1vRHMVHljR_yqM3QicLxAlXbXbrninACov2dRr0UcftGkkKgNHBDfBNxqvutp0uEdQ/pub?start=false&loop=false&delayms=3000&slide=id.g273ba00e4dc_0_122) — GopherCon 2025
- [*Beloved Functional Programming*](https://joohyung-park.my.canva.site/beloved-functional-programming-en) — liftIO 2025
- *Domain Modeling Made Functional* — In-house talk, Doctor Palette team, 2021
- *Nubes on NCC: Lessons Learnt from the Migration of an MSA Storage Service onto K8S* — Live session, NAVER Engineering Day 2020
- *네이버에서 분산플랫폼 개발자로 일한다는 것* (Working as a Distributed Platform Developer at NAVER) — Live session, NAVER Open Class 2019
- *DDZTrace: An Online Semantic-aware Block Tracing Tool* — Poster, USENIX FAST 2016


## Education

### M.S., Electrical and Computer Engineering, Sungkyunkwan University
`Sep 2014 – Aug 2016`

Advisor: Prof. Jin-Soo Kim

### B.S., Semiconductor System Engineering, Sungkyunkwan University
`Mar 2007 – Sep 2014`


## Military Service

### Sergeant, 5th Signal Group, ROK Defense Communication Command
`May 2011 – Feb 2013`

---

# 박주형
Software Engineer

Seoul, KR | joohyung.park@on-the-ground.org | [Linktree](https://linktr.ee/joohyung.park) | [Github](https://github.com/on-the-ground) | [LinkedIn](https://www.linkedin.com/in/joohyung-park-47333ab2/)

## 요약

분산 시스템과 복잡한 도메인 모델링을 다뤄온 개발자입니다. NAVER와 EMR에서 8년간 실무를 했고, 이후 기술 서적 편역과 오픈소스 언어·런타임 개발을 이어오고 있습니다. NAVER에서는 100PB+ 오브젝트 스토리지 플랫폼을 구축·이관했고, 위버케어(닥터팔레트 EMR)에서는 3~6개월마다 개정되는 1,000쪽 분량의 건강보험 청구 도메인을 재설계했습니다.

## 기술 스택

- **Languages:** Go, TypeScript, JavaScript, Kotlin, Java, Python
- **Data / Messaging:** MySQL, PostgreSQL, Redis, MongoDB, Kafka
- **Infra:** Kubernetes, Helm, Consul, Datadog
- **Systems:** Linux 커널 I/O 스택, eBPF·ftrace·perf 트레이싱
- **Concepts:** DDD, Event-Driven Architecture, Stream Processing

## 경력

### Weavrcare | Backend Developer, Doctor Palette EMR | 2021.01 – 2024.01

건강보험 청구 시스템 재설계 및 배치 파이프라인 최적화

- 1,000쪽 분량의 청구 작성요령을 bounded context 단위로 분리하고, ADT로 불필요한 추상 없이 청구 규칙을 TypeScript 타입에 인코딩해 3~6개월 주기 개정의 영향 범위 격리
- ViewModel 기반 GraphQL 스키마를 설계해 도메인 로직과 UI 관심사 분리
- 멀티테넌트 환경의 인메모리 청구 배치를 Node.js Stream 아키텍처로 전환해, 청구 건당 메모리를 100MB에서 5MB 미만으로 줄이고 청구 집중 시기의 OOM 해소

### NAVER | Storage Platform Developer, Nubes | 2016.09 – 2021.01

100PB 오브젝트 스토리지 플랫폼 구축 및 이관

- 레거시 분산 스토리지의 100PB 데이터와 수십억 건 메타데이터를 Shadow-write / Dual-read로 Nubes에 서비스 무중단 이관
- 전사 KV 캐시 장애가 Gateway 연쇄 장애로 번진 상황에서 Gateway rate limiting과 읽기 트래픽의 전용 클러스터 절체로 복구하고, 재발 방지를 위한 back pressure 아키텍처 설계
- 수백 개 MSA 인스턴스의 long polling으로 인한 Consul 병목을 진단하고, 계층적 이벤트 전파 구조로 리팩토링해 오케스트레이터 과부하 해소
- VM 기반 배포 환경을 Kubernetes/Helm 기반 MSA 운영 환경으로 전환

### Subsea Cable Language | 감사 가능한 에이전트 워크플로를 위한 DSL 및 런타임 
`2026 – 현재` | [__C Lang](https://4gentsinc.github.io/subsea_cable_webpages/)

수행 과정의 추적·감사가 필수인 고책임 도메인(금융, 대규모 데이터 마이그레이션)에서 에이전트의 워크플로를 관리하는 언어

- 선언적 계획(`.vyg`)을 lazy deduction으로 DAG/Stream에 전개해, 실행 중에도 reduction rule 수정 지원
    
- 에이전트의 의도(Goal)와 실제 연산(Leaf) 간 계보를 불변으로 기록해 감사 시 추적 지원
    
- 목적 지향 goal space와 수단 지향 host를 분리하고 goal의 arity·cardinality를 명세해, 에이전트 폭주를 시스템 레벨에서 방지

### Codeit | Node.js Backend Lead Instructor (Contract) | 2025.11 – 2025.12

- 비전공자 대상 Node.js 백엔드 부트캠프 주강사로서 강의 내용 설계, 코드 리뷰·평가 총괄

### 지은이온더그라운드 (제이펍) | Technical Translator | 2024.06 – 2025.11

- Domain Modeling Made Functional 한국어판 편역. F# 원서의 전체 예제를 Kotlin·TypeScript로 재작성하는 조건으로 원저자·PragProg·제이펍과 직접 협의해 출판
- 편역 과정에서 익힌 Arrow-kt effect handler 패턴을 오픈소스 Effect-ive Programming으로 확장

## 개인 프로젝트 및 오픈소스

### Agent Harness Protocol | 에이전트 하네스 공통 추상 포트
`Sep 2026 – Present` · [PyPI](https://pypi.org/project/agent-harness-protocol/)

에이전트 하네스에 작업을 위임하는 비즈니스용 포트. Kotlin 0.2.3 계약의 Python 구현.

- Kotlin AHP 0.2.3 계약을 Python async API로 포팅 (async with, AsyncIterator, frozen dataclass)
- 종료 상태 4종 구분 (Completed/Failed/Cancelled/Unresolved), 사용량·출력에서 None과 0/빈 값 분리
- 실행·저장소 경계에서 관측한 증거로 검증하는 58개 conformance 시나리오 작성 (수락·수명주기·상호작용·정리·영속성·실행 제한 등)
- 프로토콜·테스트만 PyPI 배포, LangGraph 어댑터는 별도 패키지로 분리해 지원 범위 문서화

### **Effect-ive Programming:** 
JVM, JS, Go 환경에서 effect와 capability를 전용 핸들링 액터에 위임하는 라이브러리
    
### **Event Streaming System:** 
Python, Bytewax 기반 실시간 스트림 프로세서 프로토타입
    
### **Strbench:** 
범용 스토리지 대상 랜덤 부하 생성 및 벤치마크 도구 (Go)
    
### **DDZ on eBPF:** 
eBPF 기반 사용자 정의 I/O 트레이싱 (Go / C)
    

## 발표 및 저술

- [Effect_ive Go](https://docs.google.com/presentation/d/e/2PACX-1vRHMVHljR_yqM3QicLxAlXbXbrninACov2dRr0UcftGkkKgNHBDfBNxqvutp0uEdQ/pub?start=false&loop=false&delayms=3000&slide=id.g273ba00e4dc_0_122): GopherCon 2025
- [Beloved Functional Programming](https://joohyung-park.my.canva.site/beloved-functional-programming-en): liftIO 2025
- Domain Modeling Made Functional: 닥터팔레트 팀 사내 발표, 2021
- Nubes on NCC: Lessons Learnt from the Migration of an MSA Storage Service onto K8S: NAVER Engineering Day 2020 라이브 세션
- 네이버에서 분산플랫폼 개발자로 일한다는 것: NAVER Open Class 2019 라이브 세션
- DDZTrace: An Online Semantic-aware Block Tracing Tool: USENIX FAST 2016 포스터

## 학력

- **성균관대학교 전자전기컴퓨터공학과 석사** | 2014.09 – 2016.08 (지도교수: 김진수)
- **성균관대학교 반도체시스템공학과 학사** | 2007.03 – 2014.09

## 병역

- **국군지휘통신사령부 제5정보통신단 · 병장** | 2011.05 – 2013.02
