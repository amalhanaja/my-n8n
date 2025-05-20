# n8n Deployment with Docker Compose

## Quickstart

####  1. Clone repository
```bash
git clone git@github.com:amalhanaja/my-n8n.git
```
#### 2. Create `.env`. You can take a look for `example.env` for example environment variable
#### 3. Start services
```bash
docker compose up -d
```

---

## 📦 Components

| Service       | Description                                                                 |
|---------------|-----------------------------------------------------------------------------|
| `n8n`         | Workflow automation platform                                                |
| `Cloudflared` | Secure tunnel to expose `n8n` publicly (no need to open ports!)             |

---

## How to update version
```bash
# Pull latest version
docker compose pull

# Stop and remove older version
docker compose down

# Start the container
docker compose up -d
```