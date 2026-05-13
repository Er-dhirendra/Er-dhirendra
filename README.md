<div align="center">

# Dhirendra Kumar Kashyap

### Senior Software Engineer · Distributed Systems · Functional Scala

[![LinkedIn](https://img.shields.io/badge/LinkedIn-dkashyap95-0077B5?style=flat&logo=linkedin)](https://www.linkedin.com/in/dkashyap95/)
[![GitHub](https://img.shields.io/badge/GitHub-Er--dhirendra-181717?style=flat&logo=github)](https://github.com/Er-dhirendra)
[![Email](https://img.shields.io/badge/Email-dkkashyap.dev@gmail.com-D14836?style=flat&logo=gmail)](mailto:dkkashyap.dev@gmail.com)
[![Location](https://img.shields.io/badge/📍-Bengaluru,_India-green?style=flat)](https://github.com/Er-dhirendra)

</div>

---

## 👨‍💻 About Me

10+ years building **high-throughput distributed systems** on the JVM.
I specialise in **functional Scala**, **event-driven architectures**, and
**real-time data pipelines** that handle millions of events at scale.

Currently a **Lead Software Engineer at Avlino**, where I design and
deliver backend systems using ZIO, Akka/Pekko, Kafka, and Spark.

I believe the best code is code that **reveals intent, handles failure
explicitly, and scales without surprises**.

---

## 🛠️ Core Stack

| Layer | Technologies |
|---|---|
| **Languages** | Scala 3, Rust, Bash |
| **Functional FP** | ZIO 2, Cats Effect, FS2 |
| **Reactive / Actor** | Akka, Pekko, Akka Streams |
| **Streaming** | Apache Kafka, ZIO Kafka, Spark Streaming |
| **HTTP** | ZIO HTTP, Play Framework, Pekko HTTP |
| **Data** | Apache Spark, PostgreSQL, MongoDB, Redis |
| **Infra** | Docker, Kubernetes, Linux, CI/CD |
| **Patterns** | CQRS, Event Sourcing, DDD, Hexagonal |

---

## 🚀 Featured Projects

### 🏢 [ZIO Attendance Platform](https://github.com/Er-dhirendra/attendance-system)
> **Production-grade attendance management system**

Event-driven microservice built with ZIO 2, ZIO HTTP, Kafka, and
PostgreSQL. Full CQRS pattern — every check-in/check-out publishes
a domain event to Kafka for downstream consumers.

```
ZIO HTTP → AttendanceService → KafkaEventPublisher → Kafka
                ↓
         PostgreSQL (write model)
```

**Stack:** `ZIO 2` `ZIO Kafka` `ZIO HTTP` `PostgreSQL` `Docker`  
**Highlights:** Domain-driven design · Type-safe errors · Zero null · Pure FP

---

### ⚙️ [Scala Design Patterns](https://github.com/Er-dhirendra/scala-design-pattern)
> **GoF + FP patterns implemented in idiomatic Scala 3**

All 23 GoF patterns + functional patterns (Monad, Lens, Type Class,
Tagless Final) with real-world use cases and when-to-use guidance.

**Stack:** `Scala 3` `Cats` `ZIO`

---

### 📐 [SOLID Principles in Scala](https://github.com/Er-dhirendra/scala-SOLID-principle)
> **SOLID demonstrated with functional and OOP Scala**

Each principle shown with bad → good examples, explaining
how Scala's type system enforces what Java needs discipline for.

**Stack:** `Scala 3`

---

## 🏗️ Architecture Thinking

```
What I design:

  ┌─────────────────────────────────────────────────────┐
  │           Event-Driven Microservices                │
  │                                                     │
  │  HTTP API → Domain Service → Event Publisher        │
  │                ↓                    ↓               │
  │           Write DB (PG)        Kafka Topic          │
  │                                     ↓               │
  │                            Consumers (N services)   │
  │                              Projections            │
  │                              Notifications          │
  │                              Analytics              │
  └─────────────────────────────────────────────────────┘

Principles I care about:
  ✦ Make illegal states unrepresentable (ADTs + sealed traits)
  ✦ Errors are values (ZIO, Either — never throw)
  ✦ Effects at the edges, pure core
  ✦ Services as ZLayer — testable by construction
```

---

## 📊 Currently Building

```
 ⬜ Distributed Rate Limiter   — ZIO + Redis, token bucket algorithm
 ⬜ Event Sourcing Platform     — Kafka as event store, ZIO Streams projections
 ⬜ Spark Performance Cookbook  — Real benchmarks, skew handling, Tungsten
 🔄 Attendance Platform         — Adding PostgreSQL, Swagger, full test suite
```

---

## 📝 Engineering Principles

> *"Make it work, make it right, make it fast — in that order."*

- **Type safety over documentation** — if it compiles, constraints are encoded
- **Explicit over implicit** — ZLayer wiring beats magic DI frameworks  
- **Fail fast, recover intentionally** — supervision trees, not try/catch everywhere
- **Data pipelines are code** — treat Spark jobs with same rigour as services

---

## 📈 GitHub Activity

<div align="center">
<a href="http://www.github.com/Er-dhirendra"><img src="https://github-readme-streak-stats.herokuapp.com/?user=Er-dhirendra&stroke=ffffff&background=1c1917&ring=0891b2&fire=0891b2&currStreakNum=ffffff&currStreakLabel=0891b2&sideNums=ffffff&sideLabels=ffffff&dates=ffffff&hide_border=true" /></a>
</div>

---

## 🤝 Open To

- **Consulting** on distributed Scala systems, Kafka architecture, ZIO migration
- **Collaborating** on functional Scala open source
- **Discussing** system design, FP patterns, Scala 3 internals

📬 **dkkashyap.dev@gmail.com**

---

<div align="center">

*"First deserve, then desire."*

</div>
---
