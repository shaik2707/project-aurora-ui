🖥️ Project Aurora — Multimodal Device UI Platform
> Frontend interfaces for a distributed LLM-powered platform serving screen-based devices at scale.
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![React](https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=black)
![AWS](https://img.shields.io/badge/AWS_EKS-FF9900?style=flat&logo=amazonaws&logoColor=white)
---
Overview
Project Aurora is a multimodal LLM service platform that renders intelligent interfaces across screen-based device ecosystems. My role focused on the frontend architecture — designing and building the UI layer that translates complex distributed system states into intuitive, accessible user experiences for developers and device operators.
The platform processes 12M+ records per day on AWS EKS, with frontend data delivery optimized for low-latency rendering and real-time state synchronization.
---
The Problem
Device operators and developers needed a unified interface to interact with a distributed backend processing millions of multimodal events daily. Existing tooling was fragmented, with no consistent UI layer — making it hard to monitor device states, trigger actions, or debug failures in real time.
---
My Approach
Designed a component-driven frontend architecture in TypeScript and React, applying Factory, Strategy, and Observer design patterns for extensibility and maintainability
Built real-time rendering services that consume distributed backend events and surface them cleanly in the UI
Collaborated with cross-disciplinary engineers to align frontend data contracts with backend API design
Followed web security best practices including CSP headers, secure token handling, and input sanitization
---
Architecture
```
┌─────────────────────────────────────────┐
│           React Frontend (TS)           │
│  ┌──────────┐  ┌──────────┐  ┌───────┐ │
│  │ Device   │  │ Event    │  │ Debug │ │
│  │ Dashboard│  │ Stream   │  │ Panel │ │
│  └──────────┘  └──────────┘  └───────┘ │
└────────────────────┬────────────────────┘
                     │ REST / WebSocket
┌────────────────────▼────────────────────┐
│         FastAPI Microservices           │
│              (AWS EKS)                  │
│         12M+ records / day              │
└─────────────────────────────────────────┘
```
---
Key Results
Metric	Result
Daily records processed	12M+
Performance improvement	30% via algorithm optimization
Teams unblocked	3 cross-functional teams
Code coverage	>90% (SonarQube)
---
Tech Stack
Layer	Technology
Frontend	TypeScript, JavaScript, React
Backend	Python, FastAPI
Infrastructure	AWS EKS, Docker, Kubernetes
CI/CD	GitLab CI/CD, Blue/Green Deployment
Observability	OpenTelemetry, Prometheus, Grafana
---
Lessons Learned
Designing frontend systems for distributed backends requires careful contract alignment — OpenAPI specs were essential to keeping frontend and backend teams in sync
Observer pattern proved critical for real-time UI updates without polling overhead
Web security considerations (CORS, CSP, token expiry) need to be first-class concerns, not afterthoughts
---
Contact
Fazal Shaik · LinkedIn · fazal.shaik2025@gmail.com
