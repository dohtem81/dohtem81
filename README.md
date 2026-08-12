# Piotr Pedziwiatr  
**Software & Systems Engineer – Autonomy, Simulation, AI & Real-Time Systems**

I build software that directly controls physical reality.

For the past 18+ years, I have designed and deployed **real-time control systems, industrial automation platforms, AI-driven machine vision, and large-scale data architectures** operating in safety-critical, high-throughput production environments.

My work lives at the intersection of:

- **Control theory & real-time systems**
- **Physics-based simulation & modeling**
- **Autonomy & robotics foundations**
- **Machine vision & applied AI**
- **High-reliability production software**

I currently lead multidisciplinary engineering teams building **industrial AI, automation, and data platforms**, while actively developing **simulation and autonomy software** in my personal projects.

---

## 🧠 Core Technical Focus

- Real-time systems & control loops (PID, state estimation, sensor fusion)
- Physics-based simulation & rigid body dynamics
- Autonomy & robotics foundations
- Machine vision & deep learning (TensorFlow, Keras)
- Distributed systems & data platforms
- High-throughput telemetry & observability pipelines

**Languages:** C++, Python, C#, SQL  
**Domains:** Robotics, autonomy, industrial automation, simulation, AI, manufacturing systems  

---

## 🚀 Featured Projects

### AISprinkler — Safety-First Local LLM Agent for Smart Irrigation

**AISprinkler** is a personal portfolio project exploring how Large Language Models can be used responsibly in **real-world physical control systems**.

Instead of treating the LLM as a black-box suggestion engine, this project implements a **hybrid deterministic + probabilistic architecture**:
- Hard safety and policy rules (stored in `PROMPTS_AND_RULES.md`) always take precedence.
- A local LLM (via Ollama) generates intelligent 24-hour irrigation schedule adjustments based on weather data and baseline schedules.
- Every recommendation includes a **confidence score**. Changes above a threshold (e.g. 85) can be auto-applied; lower-confidence suggestions trigger review and guarded retry logic.

#### Key Highlights
- **Local-first design** — Fully supports Ollama (no paid API required). Currently tested with Llama 3.2 / Qwen3 models.
- **Strong traceability & auditability** — Every LLM call, input context, raw response, confidence score, and final decision is logged with prompt versioning for full replay and governance.
- **Confidence-gated actuation** with deterministic rule enforcement before any physical action.
- Modern, production-minded stack: **FastAPI + Celery + PostgreSQL + Redis + Docker Compose**, with clean architecture and extensive design documentation.

#### Why This Project Matters
Most LLM portfolio projects are simple chat interfaces or RAG systems. AISprinkler demonstrates a more ambitious pattern: using a local LLM as a **cautious reasoning layer** inside a safety-critical loop — similar to approaches used in robotics and autonomous systems, but applied to everyday home automation (smart sprinkler control).

This project grew out of a real pain point: manually managing my yard irrigation schedule. It serves as a practical experiment in making LLM-driven decisions reliable, explainable, and safe for the physical world.

**Status**: Concept & scaffolding phase — strong architecture and documentation complete, core LLM integration with Ollama in progress.

**Tech Stack**: Python, FastAPI, LangChain, Ollama, PostgreSQL, Redis, Celery, Docker

👉 https://github.com/dohtem81/AISprinkler

---

### FlightTracker

Real-time distributed flight tracking system with Cassandra backend. Built to explore high-ingest NoSQL patterns using live aircraft data from the OpenSky Network.

A clean **write/read split** architecture where multiple collector services ingest aircraft state vectors in parallel and write to a Cassandra cluster, while a dedicated reader service powers an interactive Leaflet web frontend.

The system keeps the latest known state for every aircraft (per ICAO24) and is fully containerized with Docker Compose for one-command deployment.

#### Key Features

- Grid-based parallel data collection from OpenSky Network (OAuth2 authenticated)
- Cassandra cluster optimized for high-write throughput with per-aircraft latest-state model
- Dedicated read-only FastAPI service serving aircraft positions
- Responsive Leaflet map UI showing live aircraft markers worldwide
- Multi-service Docker Compose setup (collectors + 3-node Cassandra + reader + nginx)
- Clean separation of write and read paths for scalability

👉 https://github.com/dohtem81/FlightTracker

---

### **virtDrone — Physics-Based Drone Simulation & Control Platform**
High-fidelity real-time drone dynamics simulation and flight control modeling.

- Multi-axis rigid-body physics simulation
- Propulsion & thrust curve modeling
- Closed-loop PID flight stabilization
- Sensor modeling and feedback loops
- Real-time simulation execution

👉 https://github.com/dohtem81/virtDrone

---

### **IONet — Industrial AI & Data Platform Concepts**
Exploration of real-time industrial telemetry ingestion, analytics, and AI inference pipelines.

- Streaming data ingestion
- OT → IT data bridging
- AI integration patterns
- Real-time visualization architectures

👉 https://github.com/dohtem81/IONet

---

### **Prism — Experimental Systems & Tooling**
Focused software project exploring reusable patterns for modern engineering workflows and system-level experimentation.

- Modular architecture
- Tooling and experimentation
- Rapid prototyping
- Practical engineering patterns

👉 https://github.com/dohtem81/prism

---

### RiverRaid_2026** (2026)  
Modern, server-authoritative browser-based remake of the classic 1982 River Raid game.  

Built with FastAPI + WebSocket for realtime gameplay, JWT sessions, PostgreSQL persistence for scores/leaderboards.  
Features: procedural scrolling river, fuel management + refuel stations, destructible bridges, multi-enemy types (helicopters, tanks, jets), level scaling, missile physics, persistent top-10 leaderboard.  
Includes demo gameplay GIF for quick overview.  

👉 https://github.com/dohtem81/riverraid_2026

---

## 🎯 Engineering Philosophy

I specialize in **engineering systems where software meets physics** — environments where:

- Determinism matters  
- Latency matters  
- Reliability matters  
- Observability matters  

These constraints shape how I design architectures, control systems, and simulation environments.

---

## 🔗 Connect

- **GitHub:** https://github.com/dohtem81  
- **LinkedIn:** https://www.linkedin.com/in/piotr-pedziwiatr  

---

*If you're building autonomy, robotics, simulation, or high-performance real-time systems — let's talk.*
