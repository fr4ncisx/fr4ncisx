# Hi, I'm Francisco 👋

> **Java Backend Engineer** specialized in building high-performance, enterprise-grade systems with **Spring Boot**. Currently expanding architectural boundaries into Mobile and Frontend ecosystems.

I approach software development with an engineering mindset: **predictability, scalability, and efficiency**. My core expertise lies in the Java ecosystem, where I design architectures that prioritize long-term maintainability over short-term fixes.

I actively integrate an **AI-Enhanced Workflow** (ChatGPT, Claude, Gemini) to automate scaffolding, generate unit tests, and optimize algorithms, allowing me to dedicate deep focus to complex domain logic and architectural decisions.

---

## ⚡ Current Technical Architecture

I am currently re-engineering a monolithic concept into a **Distributed Microservices Ecosystem** using **Spring Cloud**. This project serves as a proving ground for advanced cloud-native patterns:

- **Cloud-Native Infrastructure:** Orchestrating services via **Netflix Eureka** and **Spring Cloud Gateway** as the unified edge server.
- **Core Backend:** Transitioning to **Java 25** and **Spring Boot 4** to leverage Virtual Threads and Vector API.
- **Data & Caching Strategy:** Implementing **Redis** as a distributed cache to offload the database and ensure sub-millisecond response times for frequently accessed data.
- **Architectural Patterns:** Implementing **CQRS** to decouple high-performance reads from complex transactional writes.
- **Data Transport:** Moving beyond REST by implementing **GraphQL over WebSockets** for real-time state updates.

---

## 🛠️ Technology Ecosystem

I build on top of battle-tested technologies that offer stability and enterprise readiness.

| **Domain** | **Stack & Tools** |
| :--- | :--- |
| **Backend Core** | ![Java](https://img.shields.io/badge/Java_25-ED8B00?style=flat-square&logo=openjdk&logoColor=white) ![Spring Boot 4](https://img.shields.io/badge/Spring_Boot_4-6DB33F?style=flat-square&logo=spring&logoColor=white) ![Spring Security 7](https://img.shields.io/badge/Spring_Security_7-6DB33F?style=flat-square&logo=springsecurity&logoColor=white) ![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white) |
| **Microservices & Cloud** | ![Spring Cloud](https://img.shields.io/badge/Spring_Cloud-6DB33F?style=flat-square&logo=spring&logoColor=white) ![Eureka](https://img.shields.io/badge/Netflix_Eureka-E535AB?style=flat-square&logo=netflix&logoColor=white) ![Gateway](https://img.shields.io/badge/Spring_Gateway-6DB33F?style=flat-square&logo=spring&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) |
| **Data & Infra** | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white) ![GraphQL](https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white) ![Swagger](https://img.shields.io/badge/Swagger-Docs-85EA2D?style=flat-square&logo=swagger&logoColor=black) |
| **Architecture** | ![Hexagonal](https://img.shields.io/badge/Architecture-Hexagonal-black?style=flat-square) ![DDD](https://img.shields.io/badge/Pattern-DDD-black?style=flat-square) ![CQRS](https://img.shields.io/badge/Pattern-CQRS-black?style=flat-square) |
| **Quality & Observability** | ![SonarQube](https://img.shields.io/badge/SonarQube-4E9BCD?style=flat-square&logo=sonarqube&logoColor=white) ![JUnit5](https://img.shields.io/badge/JUnit5-25A162?style=flat-square&logo=junit5&logoColor=white) ![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white) ![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white) |
| **Build & Utilities** | ![Maven](https://img.shields.io/badge/Maven-C71A36?style=flat-square&logo=apachemaven&logoColor=white) ![Gradle](https://img.shields.io/badge/Gradle-02303A?style=flat-square&logo=gradle&logoColor=white) ![Lombok](https://img.shields.io/badge/Lombok-BC0230?style=flat-square&logo=lombok&logoColor=white) ![MapStruct](https://img.shields.io/badge/MapStruct-black?style=flat-square) |
| **AI Productivity** | ![ChatGPT](https://img.shields.io/badge/ChatGPT-74aa9c?style=flat-square&logo=openai&logoColor=white) ![Claude](https://img.shields.io/badge/Claude-D97757?style=flat-square&logo=anthropic&logoColor=white) ![Gemini](https://img.shields.io/badge/Google_Gemini-8E75B2?style=flat-square&logo=googlegemini&logoColor=white) |
| **Frontend & Mobile** | ![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![Android](https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=android&logoColor=white) |
| **Environment** | ![IntelliJ IDEA](https://img.shields.io/badge/IntelliJ_IDEA-000000?style=flat-square&logo=intellijidea&logoColor=white) ![Windows](https://img.shields.io/badge/Windows-0078D6?style=flat-square&logo=windows&logoColor=white) ![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white) |

---

## ⚙️ The "Hidden" Engineering

Great software is defined by how it handles failure and scale. My code includes patterns learned from solving production incidents, not just framework documentation:

1.  **Idempotency & Consistency:** I implement **Idempotency Keys** to handle network retries safely and utilize **Optimistic Locking** (`@Version`) to prevent "Lost Updates" in high-concurrency endpoints.
2.  **Segregation of Duties (CQRS):** I strictly separate Write Models (Commands) from Read Models (Queries/Projections), allowing for independent scaling and optimized query performance.
3.  **DTO-Entity Separation:** I enforce boundaries between the Persistence Layer and the API Layer using **MapStruct**. This prevents accidental data leaks and decouples internal schema changes from external contracts.

---

## 🧩 Engineering Standards & Philosophy

My methodology is governed by strict protocols to ensure software longevity.

### 1. Domain-Centric Isolation (The Why)
I strictly enforce the **Ports & Adapters (Hexagonal)** pattern to protect the business logic.
- **Dependency Rule:** The Core Domain never depends on Spring or the DB.
- **Testability:** Business rules are unit-tested in isolation without mocking external IO.

### 2. Security & API Consistency
Security is not an afterthought; it is baked into the design.
- **Input Sanitization:** All incoming data is validated strictly using **Jakarta Validation** (`@Valid`, `@NotNull`) before processing to prevent injection attacks.
- **Least Privilege:** Services operate with minimum necessary permissions, and authentication is stateless via OAuth2 flows.

### 3. Code Quality & Reliability
- **Strict Typing:** I enforce strict adherence to **SOLID** principles.
- **Defensive Programming:** Implementation of centralized Global Exception Handling (`@ControllerAdvice`) to transform raw Java exceptions into standardized JSON responses (RFC 7807).
- **Zero-Warning Policy:** I treat compiler warnings as errors. A clean build is non-negotiable.

---

## 🗺️ Strategic Expansion Roadmap

My professional evolution is focused on becoming a **cross-platform architect**.

| **Domain** | **Engineering Focus** | **Status** |
| :--- | :--- | :--- |
| **Mobile (Kotlin)** | **Native Android Architecture.** Applying backend principles (Clean Architecture, SOLID) to the mobile lifecycle. Focus on Coroutines for non-blocking UI. | `[■■■■□□□□□□]` *Module Implementation* |
| **Frontend (React + TS)** | **Type-Safe Fullstack Engineering.** Leveraging **TypeScript** to enforce end-to-end type safety from the API DTOs to the React Components. | `[■■■□□□□□□□]` *Dashboard Architecture* |
| **DevOps (Kubernetes)** | **Orchestration & GitOps.** Transitioning from Docker Compose to **K8s** clusters. Focus on Self-Healing pods, Auto-Scaling strategies, and Helm charts management. | `[■■□□□□□□□□]` *Initial Roadmap* |
| **Scripting (Python)** | **Operational Automation.** Learning Python syntax to handle system scripting, file manipulation, and replace complex Bash scripts for local development tools. | `[■□□□□□□□□□]` *Syntax & Basics* |

---

<div align="center">
  <h3>📫 Let's engineer something scalable.</h3>
  <p>Open to discussions about High-Performance Java, Spring Architecture, or AI Integration.</p>
  
  <a href="https://www.linkedin.com/in/franciscosaurit/">
    <img src="https://img.shields.io/badge/Connect_on_LinkedIn-blue?style=for-the-badge&logo=linkedin" alt="LinkedIn" />
  </a>
</div>