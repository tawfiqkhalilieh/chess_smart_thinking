# Chess Smart Thinking 🎯♟️

[![Docker](https://img.shields.io/badge/Docker-Container-blue?logo=docker)](https://www.docker.com/) 
[![Next.js](https://img.shields.io/badge/Next.js-Frontend-black?logo=next.js)](https://nextjs.org/) 
[![Python](https://img.shields.io/badge/Python-ML-brightgreen?logo=python)](https://www.python.org/)
[![Go](https://img.shields.io/badge/Go-Scraper-blue?logo=go)](https://golang.org/)
[![C++](https://img.shields.io/badge/C++-Analysis-lightgrey?logo=c%2B%2B)](https://isocpp.org/)

**Chess Smart Thinking** is a multi-service, event-driven machine learning pipeline that scrapes chess.com data, analyzes it, trains a model to predict human thinking time, and provides a frontend for gameplay against the trained model.

---

## 🚀 Features

- Scrape chess.com user games using the public API.
- Analyze and label games for machine learning.
- Train a custom ML model to predict human thinking time.
- Frontend interface to play against the trained model.
- Modular, multi-service architecture for scalability and maintainability.

---

## 🏗 Architecture & Tech Stack

### Service 1: Frontend
- **Tech:** Next.js, React.js, Chess.js, TensorFlow.js, Tailwind CSS  
- Provides the user interface and gameplay experience.

### Service 2: Service Arbiter & Training
- **Tech:** Python, FastAPI, Pydantic, Redis, TensorFlow, NumPy, MongoDB  
- Coordinates services and manages ML training pipelines.

### Service 3: Data Scraper
- **Tech:** Go, Gin, Chess.com API, MongoDB, Redis  
- Fetches and stores user game data.

### Service 4: Data Analysis
- **Tech:** C++, OkAPI, MongoDB, Stockfish  
- Analyzes games, labels data, and prepares it for training.

### DevOps
- Docker & Docker Compose for containerized deployment.
- Git for version control.

### Architecture: Even drivcn architecture
![Architecture Diagram]("./images/drawio.png")

---

## ⚡ Installation

```bash
git clone git@github.com:tawfiqkhalilieh/chess_smart_thinking.git
cd chess_smart_thinking
docker compose up --build

