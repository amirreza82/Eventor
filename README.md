# LogFlow

**LogFlow** is a simple yet powerful distributed event logging system built with **Python**, **Go**, **Redis**, **RabbitMQ**, and **Vagrant**.  
This project simulates a production-like event flow environment, ideal for experimenting with message queues, caching, and scalable microservice communication.

---

## 🚀 Features

- 🔁 **Event-based Architecture** using RabbitMQ
- 🐍 Producer and consumer microservices written in Python
- 🦫 Go-based services for performance-critical parts
- 🔴 Redis for fast in-memory data access and temporary storage
- 📦 Vagrant setup for portable and isolated development environments
- 🛠️ Dockerized components for easy deployment

---

## 📁 Project Structure

```bash
logflow/
├── app-python/        # Python services (producers/consumers)
├── app-go/            # Go services (optional)
├── configs/           # Config files for services (e.g. env, Prometheus)
├── docker-compose.yml
├── Vagrantfile
├── README.md
└── ...
```

---

## ⚙️ Getting Started

1. **Clone the repository**  
   ```bash
   git clone https://github.com/yourusername/logflow.git
   cd logflow
   ```

2. **Start Vagrant** (if used):  
   ```bash
   vagrant up
   ```

3. **Start the services with Docker Compose**:  
   ```bash
   docker-compose up --build
   ```

---

## 📬 Example Use Case

- Python producer pushes log events into RabbitMQ
- Go consumer processes and stores the events into Redis
- Monitoring metrics are exposed via `/metrics` endpoints
- Prometheus and Grafana can be added to monitor message rates, errors, etc.

---

## 📈 Metrics and Observability

This system is compatible with:
- **Prometheus** – to collect custom metrics (e.g., processed events, failed requests)
- **Grafana** – to visualize metrics and set alerts

---

## 🧪 Status

✅ Initial setup complete  
🔧 Adding more endpoints and real-time event simulation  
🧠 Next: Create test scenarios and Grafana dashboards

---

## 📖 License

MIT © 2025 – Your Name

---

> ⚠️ This project is for educational and demonstration purposes. It mimics aspects of real-world event-driven systems without full production guarantees.
