# Surakshak360 🛡️

> **Unified AI Public Safety & Multi-Modal Intelligence Fusion Platform**  
> *Combating Digital Arrest Scams, Deepfake Extortion, Counterfeit Currency, and Fraud Networks across India.*

![Our Logo](cover.png)
---

## 📌 Executive Summary

**Surakshak360** is an enterprise-grade digital public safety platform designed to empower citizens and law enforcement agencies with real-time AI threat detection, cross-case intelligence fusion, and court-ready forensic evidence package generation.

By uniting **Natural Language Processing (NLP)**, **Spectral Audio Deepfake Analysis**, **Computer Vision OCR & Forgery Inspection**, and **Graph Network Analytics**, Surakshak360 bridges the gap between fragmented crime reporting and actionable law enforcement intelligence.

---

## 🌟 The Core Idea & Problem Solved

### The Problem
- **Digital Arrest & Authority Impersonation**: Fraudsters impersonate Police, CBI, ED, or Customs officials over video/voice calls, placing victims under false "digital arrest" and extorting millions of Rupees.
- **Deepfake Voice Cloning**: Generative voice cloning is used to trick family members or officials into transferring money under fake emergency scenarios.
- **Counterfeit Currency Notes**: High-quality fake Indian currency notes (FICN) circulate undetected without fast optical authentication tools.
- **Fragmented Crime Data**: Fraud cases reported across different police stations are rarely linked, allowing organized crime syndicates to operate anonymously.

### The Surakshak360 Solution
1. **Multi-Modal AI Threat Scanner**: Citizens and officers can instantly analyze suspicious text messages, deepfake voice audio recordings, counterfeit banknote photos, fake arrest warrants, and phishing links.
2. **Graph Intelligence Fusion Engine**: Automatically links isolated cases sharing telephone numbers, bank accounts, UPI handles, device signatures, or IP addresses using graph correlation networks.
3. **Geospatial Hotspot Analytics**: Clusters spatial crime patterns using density-based algorithms (DBSCAN) to allocate police patrol resources efficiently.
4. **Court-Ready Evidence Briefs**: Automatically generates PDF and JSON forensic evidence packages with mathematical risk breakdowns for court proceedings.

---

## 🚀 Key Features

| Feature Module | Technology Stack | Capabilities |
| :--- | :--- | :--- |
| **Multi-Modal AI Scanner** | Python, PyTorch, Librosa, OpenCV | Text scam detection, audio deepfake scoring, currency forgery checks, warrant OCR inspection, phishing URL risk assessment. |
| **Graph Fusion Engine** | NetworkX, Neo4j Graph Schema | Ingests case indicators, builds entity relationship graphs (`Person`, `Account`, `PhoneNumber`, `Device`), detects fraud rings. |
| **Geospatial Crime Map** | Leaflet / Mapbox, Scikit-Learn DBSCAN | Heatmap rendering and cluster identification for geographic fraud concentration. |
| **Investigation Console** | Next.js 16, TailwindCSS | Case queue management, court evidence brief export, interactive graph node canvas for officers. |
| **Backend Gateway** | FastAPI, Supabase Cloud DB | JWT authentication, RBAC (Citizen, Officer, Admin), case CRUD, file upload presigned workflows. |

---

## 🌐 Microservice Port Architecture

Surakshak360 operates as a multi-tier microservice ecosystem:

```
                  ┌─────────────────────────────────────┐
                  │    Next.js Web Frontend (Port 3000) │
                  └──────────────────┬──────────────────┘
                                     │
         ┌───────────────────────────┼───────────────────────────┐
         ▼                           ▼                           ▼
┌─────────────────┐         ┌──────────────────┐        ┌──────────────────┐
│ Backend Gateway │         │ Scam Intel AI    │        │ Vision AI        │
│   (Port 8000)   │         │   (Port 8001)    │        │   (Port 8002)    │
└────────┬────────┘         └──────────────────┘        └──────────────────┘
         │
         ▼
┌──────────────────┐
│ Graph Fusion AI  │
│   (Port 8003)    │
└──────────────────┘
```

| Service | Port | Endpoint URL | Description |
| :--- | :---: | :--- | :--- |
| **Frontend Web App** | `3000` | `http://localhost:3000` | Next.js citizen & officer dashboards |
| **Backend Gateway** | `8000` | `http://localhost:8000/v1` | Auth, User/Case DB Bridge (Supabase) |
| **Scam Intelligence** | `8001` | `http://localhost:8001` | NLP text, Indic translation, Audio deepfake |
| **Vision AI Service** | `8002` | `http://localhost:8002` | Currency OCR, Document forgery, QR code |
| **Intelligence Engine**| `8003` | `http://localhost:8003` | Graph correlation, Fusion, Hotspots, Evidence |

---

## ⚙️ Quickstart & Local Setup

### Prerequisites
- **Python 3.10+**
- **Node.js 18+** & npm
- Tesseract OCR (Optional, for document scanning)

### 1. Clone & Install Dependencies
```bash
# Clone the repository
git clone https://github.com/Surakshak360/surakshak360.git
cd surakshak360

# Install backend Python dependencies
pip install -r backend/requirements.txt
pip install -r scam-intelligence/requirements.txt
pip install -r vision/requirements.txt
pip install -r intelligence/requirements.txt

# Install frontend Node dependencies
cd frontend
npm install
cd ..
```

### 2. Launch All Microservices
Run the automated orchestrator script in the project root:

```bash
python start-services.py
```
*This starts ports 8000, 8001, 8002, and 8003 automatically.*

### 3. Launch Frontend Web App
Open a separate terminal:

```bash
cd frontend
npm run dev
```

Visit **`http://localhost:3000`** in your browser.

---

## 📚 Technical Documentation & Guides

For deep dives into codebase architecture and repo decomposition, see:

- 🏛️ **[ARCHITECTURE.md](https://github.com/surakshak360/docs/blob/main/ARCHITECTURE.md)**: Deep dive into system architecture, data pipelines, graph schemas, and fusion formulas.
- 📁 **[ORGANIZATION.md](https://github.com/surakshak360/docs/blob/main/ORGANIZATION.md)**: Detailed breakdown of repository structure, microservices responsibility matrix, and inter-service APIs.

---

## 🤝 Contributor & Project Details

- **Project Team**: Surakshak360 Engineering Team
- **Repository**: [github.com/surakshak360](https://github.com/surakshak360)
- **License**: MIT License

Members and their contributions:
- **[Madhumita S](https://github.com/Madhumita-05)**: Frontend, Intelligent Feature Fusion and Spatial Mapping
- **[Shobhana S](https://github.com/Shobhanashankar)**: Audio spectral analysis layer and Vision-based counterfeit detection
- **[Sriram S V](https://github.com/IamRasengan)**: Backend development and Data layer formation
- **[Gautham R](https://github.com/gautham-here)**: Integration, cloud deployment and testing

---
*Built for digital public safety, intelligence fusion, and crime prevention.*
