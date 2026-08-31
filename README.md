# Piotr Pedziwiatr

**Engineering Leader · Real-Time Systems · Industrial AI · Autonomy**

I lead multidisciplinary engineering teams building industrial AI, automation, and data platforms — and I stay close to the technical work.

For 18+ years I’ve designed and shipped **real-time control systems, machine vision, physics-based simulation, and high-reliability production software** in safety-critical environments. My focus sits at the intersection of software, physics, and operational reality.

---

## What I Care About

- Systems where latency, determinism, and reliability actually matter
- Clean service boundaries and graceful degradation under failure
- Making complex technical decisions understandable to teams and stakeholders
- Keeping technical judgment sharp while leading people and delivery

**Languages:** C++, Python, C#, SQL  
**Domains:** Real-time systems, industrial automation, autonomy & robotics, machine vision, distributed data platforms

---

## Featured Work

### Prism — Real-Time Multilingual Chat Platform
Server-side translation that never blocks the conversation.

Messages are delivered immediately. Translation runs asynchronously via a decoupled worker and is pushed live as an update. When the LLM provider is unavailable, the original message stays fully usable and the status is surfaced to clients.

**Highlights**
- FastAPI + WebSocket + Celery + RabbitMQ + PostgreSQL + Redis
- Graceful degradation, DLQ, rate limiting, quotas, and abuse protection
- Admin metrics (latency, cost, success rates) + structured logging + lightweight distributed tracing
- Docker-first, clean architecture, extensive design documentation

👉 [github.com/dohtem81/prism](https://github.com/dohtem81/prism)

---

### AISprinkler — Safety-First Local LLM for Physical Control
Exploring how LLMs can sit inside real-world control loops without becoming a liability.

Hybrid architecture: hard deterministic safety rules always win. A local LLM (Ollama) proposes schedule adjustments with confidence scores. High-confidence changes can be applied; lower-confidence ones require review. Full audit trail of every prompt, response, and decision.

**Why it matters**  
Most LLM demos are chat or RAG. This one treats the model as a cautious reasoning layer inside a safety-critical actuation path.

👉 [github.com/dohtem81/AISprinkler](https://github.com/dohtem81/AISprinkler)

---

### FlightTracker — High-Ingest Real-Time Aircraft Tracking
Write/read split architecture using live OpenSky Network data and Cassandra.

Multiple collectors ingest in parallel; a dedicated reader serves a live Leaflet map. Designed for high write throughput and clean separation of concerns. Fully containerized.

👉 [github.com/dohtem81/FlightTracker](https://github.com/dohtem81/FlightTracker)

---

### virtDrone — Physics-Based Drone Simulation & Control
Real-time rigid-body dynamics, thrust modeling, closed-loop PID stabilization, and sensor feedback loops.

👉 [github.com/dohtem81/virtDrone](https://github.com/dohtem81/virtDrone)

---

### IONet — Industrial Telemetry & AI Concepts
Patterns for streaming OT→IT data, real-time analytics, and AI inference in industrial environments.

👉 [github.com/dohtem81/IONet](https://github.com/dohtem81/IONet)

---

## Engineering Philosophy

I design systems where software meets the physical world:

- Determinism matters  
- Latency matters  
- Reliability matters  
- Observability matters  

These constraints shape architecture decisions, team practices, and what “done” actually means.

---

## Connect

- GitHub: [github.com/dohtem81](https://github.com/dohtem81)  
- LinkedIn: [linkedin.com/in/piotr-pedziwiatr](https://www.linkedin.com/in/piotr-pedziwiatr)

---

*Building autonomy, industrial AI, or high-reliability real-time systems? Let’s talk.*