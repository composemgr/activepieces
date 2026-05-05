## 👋 Welcome to activepieces 🚀

Open-source business automation platform with visual workflow builder

## 📋 Description

Open-source business automation platform with visual workflow builder

## 🚀 Services

- **activepieces**: activepieces/activepieces:latest

### Infrastructure Components

- **activepieces-db**: Postgres database


## 📦 Installation

### Option 1: Quick Install
```bash
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/activepieces/main/docker-compose.yaml" -o compose.yml
```

### Option 2: Git Clone
```bash
git clone "https://github.com/composemgr/activepieces" ~/.local/srv/docker/activepieces
cd ~/.local/srv/docker/activepieces
docker compose up -d
```

### Option 3: Using composemgr
```bash
composemgr install activepieces
```

## 🔧 Configuration

### Environment Variables

```shell
TZ=America/New_York
DB_USER_NAME=activepieces
```

See `docker-compose.yaml` for complete list of configurable options.

## 🌐 Access

- **Web Interface**: http://172.17.0.1:8092

## 📂 Volumes

- `./volumes/data/activepieces` - Data storage
- `./volumes/config/activepieces` - Data storage
- `./volumes/data/db/postgres/activepieces` - Data storage

## 🔐 Security

- Change all default passwords before deploying to production
- Use strong secrets for all authentication tokens
- Configure HTTPS using a reverse proxy (nginx, traefik, caddy)
- Regularly update Docker images for security patches
- Backup your data regularly

## 🔍 Logging

```shell
docker compose logs -f activepieces
```

## 🛠️ Management

```bash
# Start services
docker compose up -d

# Stop services
docker compose down

# Update to latest images
docker compose pull && docker compose up -d

# View logs
docker compose logs -f

# Restart services
docker compose restart
```

## 📋 Requirements

- Docker Engine 20.10+
- Docker Compose V2+

## 🤝 Author

🤖 casjay: [Github](https://github.com/casjay) 🤖  
🦄 composemgr: [Github](https://github.com/composemgr) 🦄
