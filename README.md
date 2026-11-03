# Ecommerce Microservices Architecture

Scalable e-commerce platform with 8 microservices (Identity, Customer, Catalog, Cart, Inventory, Order, Payment, Notification). Uses API Gateway, Saga checkout to prevent overselling, Redis/CDN cache, Elasticsearch, K8s autoscaling, event-driven outbox pattern, and PCI-compliant secure payments.

## Architecture Overview
- **Pattern:** Microservices + Database-per-service
- **Communication:** REST via API Gateway + Async Events via Kafka/RabbitMQ
- **Checkout Flow:** Saga Pattern (Order -> Reserve Stock -> Payment -> Confirm)
- **Stack:** React/Next.js, Spring Boot/FastAPI, PostgreSQL, Redis, Elasticsearch, S3, Kubernetes

## Documents
- Full architecture doc in `/docs` folder
