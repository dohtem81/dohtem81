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

### FlightTracker

Real-time distributed flight tracking system with Cassandra backend. Built to explore high-ingest NoSQL patterns using live aircraft data from the OpenSky Network.

## Overview

A clean **write/read split** architecture where multiple collector services ingest aircraft state vectors in parallel and write to a Cassandra cluster, while a dedicated reader service powers an interactive Leaflet web frontend.

The system keeps the latest known state for every aircraft (per ICAO24) and is fully containerized with Docker Compose for one-command deployment.

## Key Features

- Grid-based parallel data collection from OpenSky Network (OAuth2 authenticated)
- Cassandra cluster optimized for high-write throughput with per-aircraft latest-state model
- Dedicated read-only FastAPI service serving aircraft positions
- Responsive Leaflet map UI showing live aircraft markers worldwide
- Multi-service Docker Compose setup (collectors + 3-node Cassandra + reader + nginx)
- Clean separation of write and read paths for scalability

👉 https://github.com/dohtem81/FlightTracker

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

### RiverRaid_2026** (2026)  
Modern, server-authoritative browser-based remake of the classic 1982 River Raid game.  

Built with FastAPI + WebSocket for realtime gameplay, JWT sessions, PostgreSQL persistence for scores/leaderboards.  
Features: procedural scrolling river, fuel management + refuel stations, destructible bridges, multi-enemy types (helicopters, tanks, jets), level scaling, missile physics, persistent top-10 leaderboard.  
Live playable demo: https://riverraid-2026.onrender.com/  
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
