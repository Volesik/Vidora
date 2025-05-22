# Vidora
**Vidora** is a modern cinema platform designed for exploring movies, series, and animations.

## 🚀 Features
- 🔐 Modular Authentication System (OAuth / IdentityServer)
- 🎞️ Media catalog: Movies, Series, Cartoons
- 📡 Real-time communication via SignalR
- 🧠 Intelligent Search with Elasticsearch
- ⏱️ Background processing with Hangfire
- 📈 Monitoring & Metrics with Grafana + Prometheus
- 🐳 Fully containerized architecture
- 🔁 Event-driven communication with Apache Kafka

---

## 🧰 Tech Stack

| Layer              | Technology                                                                 |
|-------------------|-----------------------------------------------------------------------------|
| Backend API        | ![.NET 9](https://img.shields.io/badge/.NET-9.0-blue) ASP.NET Core Web API |
| Frontend           | ![Angular](https://img.shields.io/badge/Angular-19.2.0-red) Angular            |
| Database           | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-17-blue)             |
| Background Jobs    | ![Hangfire](https://img.shields.io/badge/Hangfire-Jobs-informational)      |
| Auth Service       | ASP.NET Identity / IdentityServer                                          |
| Realtime           | ![SignalR](https://img.shields.io/badge/SignalR-Realtime-brightgreen)      |
| Logging & Search   | ![Elasticsearch](https://img.shields.io/badge/Elasticsearch-Search-yellow) |
| Monitoring         | ![Grafana](https://img.shields.io/badge/Grafana-Dashboard-orange)          |
| Messaging          | ![Kafka](https://img.shields.io/badge/Kafka-Events-ff69b4)                 |
| Containerization   | ![Docker](https://img.shields.io/badge/Docker-Compose-blueviolet) 

---

## 🗺️ Roadmap

### Phase 1: Project Initialization & Architecture Design
✅ **Set up GitHub repo with `README.md`, `.gitignore`**<br>
✅ **Set up solution folder structure**<br>

### Phase 2: Infrastructure & Docker Setup
✅ **Create `docker-compose.yml` with containers for PostgreSQL, Kafka, Elasticsearch, Grafana, etc.**<br>
✅ **Dockerfiles for ASP.NET API, Angular, Hangfire, Auth**<br>
✅ **Configure `.env` for shared variables**<br>

### Phase 3: Backend Foundation (.NET 9 Web API)
- [ ] Initialize ASP.NET Core project
- [ ] Setup EF Core, PostgreSQL, entities, AutoMapper, layered architecture
- [ ] Add Swagger and basic services

### Phase 4: Frontend (Angular)
- [ ] Setup Angular workspace and routing
- [ ] Implement catalog UI (list/details), responsive design
- [ ] Connect to API, setup loading/error handling

### Phase 5: Authentication & User Roles
- [ ] Implement IdentityServer or ASP.NET Identity
- [ ] JWT authentication, refresh tokens, roles
- [ ] Guard routes on frontend

### Phase 6: Kafka & Real-Time Events
- [ ] Add Kafka producer/consumer for media events
- [ ] Display viewers count with SignalR
- [ ] Create mock event publisher

### Phase 7: Hangfire & Background Jobs
- [ ] Setup Hangfire dashboard
- [ ] Add tasks like data cleanup, popularity scoring

### Phase 8: Search with Elasticsearch
- [ ] Index media in Elasticsearch
- [ ] Implement search/filter in API + Angular

### Phase 9: Monitoring & Logs
- [ ] Serilog logging to Elasticsearch
- [ ] Grafana + Prometheus for dashboards

### Phase 10: Testing & QA
- [ ] Unit/integration tests, API testing, E2E testing

### Phase 11: DevOps & CI/CD
- [ ] GitHub Actions CI/CD pipeline
- [ ] Deploy on GCP/Azure with secrets

### Phase 12: Final Touches
- [ ] Theming, internationalization, UI polish

### Optional Enhancements
- [ ] Ratings, favorites, notifications
- [ ] AI-based recommendations

---

## 📂 Project Structure (planned)
```
/Vidora
│
├── /frontend           # Angular app
├── /backend            # ASP.NET Core API
├── /auth               # Auth service (optional)
├── /hangfire           # Background jobs worker
├── /infrastructure     # Kafka, Grafana, PostgreSQL, etc.
└── docker-compose.yml  # Multi-container orchestration
```

---

## 📸 Screenshots (Coming soon...)

Stay tuned for UI previews and architecture diagrams.

---

> _"Your gateway to the cinematic universe — in code."_
