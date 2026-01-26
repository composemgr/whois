## 👋 Welcome to whois 🚀

Self-hosted whois application

## 📋 Description

Self-hosted whois application

## 🚀 Services

- **app**: dumbwareio/dumbwhois:latest

## 📦 Installation

### Option 1: Quick Install
```bash
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/whois/main/docker-compose.yaml" -o compose.yml
```

### Option 2: Git Clone
```bash
git clone "https://github.com/composemgr/whois" ~/.local/srv/docker/whois
cd ~/.local/srv/docker/whois
docker compose up -d
```

### Option 3: Using composemgr
```bash
composemgr install whois
```

## 🔧 Configuration

### Environment Variables

```shell
TZ=America/New_York
DUMBWHOIS_SITE_TITLE=DumbWhois
DUMBWHOIS_ALLOWED_ORIGINS=*
```

See `docker-compose.yaml` for complete list of configurable options.

## 🌐 Access

- **Web Interface**: http://172.17.0.1:62038

## 📂 Volumes

- `./rootfs/data` - Data storage
- `./rootfs/config` - Data storage

## 🔍 Logging

```shell
docker compose logs -f app
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
