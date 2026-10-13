---
layout: cv
title: Joohyung Park's CV
---

# Joohyung Park
Backend Engineer

Seoul, KR · [joohyung.park@on-the-ground.org](mailto:joohyung.park@on-the-ground.org) · [Linktree](https://linktr.ee/joohyung.park) · [GitHub](https://github.com/on-the-ground) · [LinkedIn](https://www.linkedin.com/in/joohyung-park-47333ab2/)


## Summary

Backend engineer working on distributed systems and complex domain modeling. 7 years of industry experience at NAVER and Weavrcare, followed by technical book translation and open-source language/runtime work. At NAVER, built and migrated a 100PB+ object storage platform. At Weavrcare (Doctor Palette EMR), redesigned the health insurance billing domain, governed by a 1,000-page guideline revised every 3–6 months.


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

### Codeit · Node.js Backend Lead Instructor (Contract)
`Nov 2025 – Dec 2025`

- Lead instructor for a Node.js backend bootcamp for non-CS majors; designed lecture content and led code reviews and assessments

### Ontheground (JPub) · Technical Translator
`Jun 2024 – Nov 2025`

- Translated *Domain Modeling Made Functional* into Korean, rewriting all F# examples in Kotlin and TypeScript
- Negotiated the rewrite with the author, PragProg, and JPub as a condition of the Korean edition
- Extended the Arrow-kt effect handler pattern learned during translation into the open-source Effect-ive Programming libraries


## Personal Projects & Open Source

### Subsea Cable · DSL and runtime for auditable agent workflows
`2026 – Present`

Workflow language for agents in high-responsibility domains (finance, large-scale data migration) where traceability and audit are required

- Lazily deduces declarative plans (`.vyg`) into DAGs/streams, allowing reduction rules to change at runtime
- Records lineage between agent intent (Goal) and executed operations (Leaf) as immutable state for audit tracing
- Separates the goal space (ends) from the host (means) and specifies goal arity and cardinality, preventing runaway agent behavior at the system level

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
