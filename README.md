# 🔄 Interactive Limit Order Book  
Mentor-**Prof. Anirban Banerjee**, IIM Ahmedabad  
**Timeline:** Dec 2024 – May 2025  

---

## 📌 Project Overview  
Developed a full-featured trading simulator that replicates modern equity exchange mechanics. The engine supports multiple order types, processes high‑throughput event streams, and delivers live order book updates for research and classroom demos.

---

## 🧩 Key Features  

- **Multi‑Order Engine**  
  - Implemented 5+ order types: Market, Limit, Immediate‑Or‑Cancel (IOC), Iceberg, Stop‑Loss.  
  - Precise order matching logic to mirror real-world exchange rules.

- **Realistic Market Simulation**  
  - Modeled order flow from 600+ simulated users.  
  - Tested across 10+ market scenarios covering varying volatility and liquidity regimes.

- **Live Order Book Updates**  
  - Bid/ask book rendered in real time via WebSockets and AJAX.  
  - Zero‑reload UI syncs seamlessly with backend matching engine.

- **High‑Performance Matching**  
  - Event‑driven architecture powered by Redis pub/sub.  
  - Sustained throughput of 10,000+ orders per minute with <2 s round‑trip latency.

- **Post‑Trade Analytics**  
  - All trades and user sessions logged in PostgreSQL.  
  - CSV export for offline strategy analysis and performance review.

---

## 🛠 Tech Stack  

- **Backend:** Django, Redis (pub/sub), PostgreSQL  
- **Realtime:** WebSockets, AJAX  
- **Data Export:** Python CSV utilities  
- **Deployment:** Docker, Docker Compose  

---

## 🚀 Impact & Next Steps  

- **Scalable Classroom Demo:** Supports live trading labs for up to 50 concurrent students.  
- **Research Platform:** Baseline for studying order‑book dynamics, algorithmic trading strategies, and latency effects.  
- **Future Enhancements:**  
  - Add more exotic order types (e.g., Stop‑Limit)  
  - Web UI performance optimizations  
  - Containerized CI/CD pipeline  

---

> “A hands‑on environment that brings exchange mechanics to life—perfect for teaching, research, and prototyping new strategies.”  
