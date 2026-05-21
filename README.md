<div align="center">

# Dhirendra Kumar Kashyap

### Lead Software Engineer · Distributed Systems · Functional Scala

[![LinkedIn](https://img.shields.io/badge/LinkedIn-dkashyap95-0077B5?style=flat&logo=linkedin)](https://www.linkedin.com/in/dkashyap95/)
[![Email](https://img.shields.io/badge/Email-dkkashyap.dev%40gmail.com-D14836?style=flat&logo=gmail)](mailto:dkkashyap.dev@gmail.com)
[![Location](https://img.shields.io/badge/📍-Bengaluru,_India-2ea44f?style=flat)](https://github.com/Er-dhirendra)

</div>

---

## 👨‍💻 About Me

10+ years building **high-throughput distributed systems** on the JVM.

I specialise in **functional Scala**, **event-driven architectures**,
and **real-time data pipelines** that handle millions of events at scale.

Currently **Lead Software Engineer at Avlino** — designing backend
systems with ZIO, Akka/Pekko, Kafka, and Apache Spark.

Publishing open-source libraries for the Scala/ZIO ecosystem — latest: [**zio-ulid**](https://github.com/Er-dhirendra/zio-ulid).

> *I believe the best code reveals intent, handles failure explicitly,
> and scales without surprises.*

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
| **Patterns** | CQRS, Event Sourcing, DDD, Hexagonal Architecture |

---

## 🚀 Featured Projects

### 🆔 [zio-ulid](https://github.com/Er-dhirendra/zio-ulid) · [![CI](https://github.com/Er-dhirendra/zio-ulid/actions/workflows/ci.yml/badge.svg)](https://github.com/Er-dhirendra/zio-ulid/actions/workflows/ci.yml)
> **Type-safe ULID generation for ZIO 2.x**

Lexicographically sortable 128-bit identifiers with production-ready layers:
`live` (SecureRandom), `monotonic` (strict ordering per millisecond), `fast`, and `deterministic` for tests.

```scala
import zio._
import zio.ulid._

ULIDGen.generate.provide(ULIDGen.live)
// e.g. 01ARZ3NDEKTSV4RRFFQ69G5FAV
```

**Stack:** `ZIO 2` `Scala 3` `Scala 2.13` `MUnit`  
**Maven:** `dev.zio %% "zio-ulid" % "0.1.0"` · [Central](https://central.sonatype.com/artifact/dev.zio/zio-ulid_3)

---

### 🏢 [ZIO Attendance Platform](https://github.com/Er-dhirendra/attendance-system)
> **Production-grade attendance management system**

Event-driven microservice with full CQRS — every check-in/out
publishes a domain event to Kafka for downstream consumers.

```
ZIO HTTP → AttendanceService → KafkaEventPublisher → Kafka Topics
                ↓                       ↓
         PostgreSQL (write)      Consumers (notify / payroll / HR)
```

**Stack:** `ZIO 2` `ZIO Kafka` `ZIO HTTP` `PostgreSQL` `Docker`  
**Highlights:** Domain-driven · Type-safe errors · Zero null · Pure FP

---

### ⚙️ [Scala Design Patterns](https://github.com/Er-dhirendra/scala-design-pattern)
> **23 GoF + Functional patterns in idiomatic Scala 3**

All patterns with real-world use cases, when-to-use guidance,
and comparisons between OOP and functional approaches.

**Stack:** `Scala 3` `ZIO` `Cats`

---

### 📊 [Spark Performance Cookbook](https://github.com/Er-dhirendra/spark-performance-cookbook)
> **Runnable tuning recipes for Spark SQL**

Seven chapters: partitioning, broadcast joins, caching, skew, AQE, Parquet vs JSON, and UDF pitfalls — each with local demos and MUnit tests.

**Stack:** `Spark 3.5` `Scala 2.13` `MUnit`

---

### 📐 [SOLID in Scala](https://github.com/Er-dhirendra/scala-SOLID-principle)
> **SOLID principles — bad vs good examples in Scala**

Shows how Scala's type system enforces what Java needs
discipline for. Each principle with clear before/after examples.

**Stack:** `Scala 3`

---

## 🏗️ Architecture Thinking

```
What I design:

  ┌──────────────────────────────────────────────────────┐
  │            Event-Driven Microservices                │
  │                                                      │
  │  HTTP API → Domain Service → Event Publisher         │
  │                ↓                    ↓                │
  │         Write DB (PG)          Kafka Topic           │
  │                                      ↓               │
  │                           Consumers (N services)     │
  │                             Projections              │
  │                             Notifications            │
  │                             Analytics                │
  └──────────────────────────────────────────────────────┘

Principles I code by:
  ✦ Make illegal states unrepresentable  (ADTs + sealed traits)
  ✦ Errors are values                    (ZIO / Either — never throw)
  ✦ Effects at the edges, pure core      (Hexagonal architecture)
  ✦ Services wired by type               (ZLayer — testable by design)
```

---

## 🔨 Currently Building

| Status | Project | Stack |
|---|---|---|
| 🔄 Active | [zio-ulid](https://github.com/Er-dhirendra/zio-ulid) — Maven Central release, docs | ZIO · MUnit · sbt-ci-release |
| 🔄 Active | Attendance Platform — PG, Swagger, tests | ZIO · Kafka · PostgreSQL |
| ⬜ Next | Distributed Rate Limiter | ZIO · Redis |
| ⬜ Planned | Event Sourcing Platform | Kafka · ZIO Streams |
| 🔄 Active | [Spark Performance Cookbook](https://github.com/Er-dhirendra/spark-performance-cookbook) — 7 chapters, CI | Spark 3.5 · Scala 2.13 |

---

## 📈 GitHub Stats

<div align="center">

<a href="http://www.github.com/Er-dhirendra"><img src="https://github-readme-streak-stats.herokuapp.com/?user=Er-dhirendra&stroke=ffffff&background=1c1917&ring=0891b2&fire=0891b2&currStreakNum=ffffff&currStreakLabel=0891b2&sideNums=ffffff&sideLabels=ffffff&dates=ffffff&hide_border=true" /></a>

</div>

---

## 🤝 Open To

- **Consulting** on distributed Scala systems, Kafka architecture, ZIO migration
- **Collaborating** on functional Scala open source (ZIO ecosystem, libraries)
- **Speaking** about ZIO, Akka internals, event-driven design

📬 **dkkashyap.dev@gmail.com** · [LinkedIn](https://www.linkedin.com/in/dkashyap95/)

---

<div align="center">

*"First deserve, then desire."*

</div>
