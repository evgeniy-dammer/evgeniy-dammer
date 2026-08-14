## Senior backend engineer, Go. High-load microservices — messaging, video streaming, payments.

I joined a messaging platform as its sole backend engineer while the acquired backend was crashing
roughly every four hours, and rebuilt it into 60+ Go microservices serving 700K registered users,
120K DAU and 10–15M messages a day across ~50 servers. Mean time between production failures went
from ~4 hours to ~2 weeks. Profiling every service, MySQL sharding, query and index work and caching
with Redis and DragonflyDB cut system load by 30% and halved response latency in several services.
I introduced observability from scratch, took 60+ services to Docker and Kubernetes, and was the
sole author of the platform's payment service and bank SDK — its first revenue stream.

Since then I have architected two greenfield products from zero to working MVP: a QR-code payment
platform designed to PCI DSS principles, and a B2B courier dispatch platform deliberately kept
outside PCI scope.

8+ years in software engineering, the last 3+ in production Go. **Most of that work lives in private
company repositories**, so what is public here is side projects rather than the systems described
above.

### Worth looking at

- **[marketplace-api](https://github.com/evgeniy-dammer/marketplace-api)** — Go REST API. JWT auth
  with a refresh-token whitelist, HashiCorp Vault for secrets, a SQL builder over the Postgres
  repositories, Jaeger tracing, Docker Compose, GitHub Actions CI.
- **[blockchain](https://github.com/evgeniy-dammer/blockchain)** — a modular blockchain
  implementation in Go.
- **[clean-architecture](https://github.com/evgeniy-dammer/clean-architecture)** — reference layout
  for a Go service with transport, business logic and persistence kept separate.
- **[ecommerce](https://github.com/evgeniy-dammer/ecommerce)** — TypeScript service, with its
  contracts in a separate repository.

Upstream: a documentation contribution to
[apache/casbin-pg-adapter](https://github.com/apache/casbin-pg-adapter) explaining how to reuse an
existing database connection — written after running into the gap while using Casbin in production.

### Stack

Go, go-zero, gRPC, PostgreSQL, MySQL, Redis, DragonflyDB, Kafka, ClickHouse, MinIO, etcd,
Prometheus, Grafana, Jaeger, Docker, Kubernetes, GitLab CI.

### Contact

[LinkedIn](https://www.linkedin.com/in/evgeniydammer) · [Telegram](https://t.me/evgeniydammer)

Based in Ashgabat (UTC+5) — full overlap with European business hours. Open to fully remote senior
backend roles.
