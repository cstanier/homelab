# HomeLab Infrastructure

Infrastructure as Code for my home media server and automation platform.

## Hardware

- **Mini PC**: Beelink Mini S13 (primary host)
- **OS**: Ubuntu Server LTS
- **Storage**: `/srv/media`, `/srv/downloads`, `/srv/configs`

## Services

- **Jellyfin**: Media server (port 8096)
- **qBittorrent**: Download manager (port 8080)
- **Sonarr/Radarr**: Media automation (planned)

## Quick Start
```bash
# Deploy services
docker-compose up -d

# Update services
git pull && docker-compose up -d
```

## Repository Structure
```
homelab/
├── docker-compose.yml      # Service definitions
├── .env.example           # Template for secrets
├── scripts/               # Setup and deployment scripts
├── configs/               # App-specific configs
└── docs/                  # Documentation
```