# Real-Time Load Testing & Observability Pipeline

A production-grade, local observability pipeline designed to simulate concurrent user loads and stream real-time telemetry metrics using **k6**, **InfluxDB**, and **Grafana**, fully orchestrated with **Docker Compose**.

---

## 📌 Overview

This project demonstrates an end-to-end performance testing and observability architecture. Instead of relying solely on post-test summaries, it ingests continuous time-series metrics during execution, enabling real-time monitoring of application stability, virtual user (VU) concurrency, and response latency.

---

## 🛠️ Tech Stack & Architecture

- **k6 (Grafana Labs)**: Distributed load testing tool simulating concurrent Virtual Users (`10 VUs`).
- **InfluxDB (TSDB)**: Time-series database optimized for real-time metric ingestion and fast query lookups.
- **Grafana**: Telemetry visualization platform querying InfluxQL with custom aggregation strategies (`mean`, `fill(previous)`).
- **Docker & Docker Compose**: Containerized multi-service orchestration with isolated bridge networking.

---

## 🚀 Getting Started

### 1. Prerequisites
- [Docker Desktop](https://www.docker.com/products/docker-desktop/) installed and running
- [k6](https://k6.io/docs/get-started/installation/) installed locally

### 2. Start the Infrastructure
Spin up the InfluxDB and Grafana containers:
```bash
docker-compose up -d
