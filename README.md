# Real-Time Load Testing & Observability Pipeline

Pipeline de testes de carga e telemetria em tempo real integrando **k6**, **InfluxDB** e **Grafana** via **Docker**.

## 🛠️ Tecnologias
- **k6**: Simulação de utilizadores virtuais simultâneos (VUs).
- **InfluxDB**: Armazenamento de métricas em séries temporais (TSDB).
- **Grafana**: Visualização de dashboards em tempo real com InfluxQL.
- **Docker Compose**: Orquestração local dos serviços.

## 🚀 Como executar

1. Subir os containers:
   ```bash
   docker-compose up -d
