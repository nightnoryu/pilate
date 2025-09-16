# :strawberry: Pilate [![Github release](https://img.shields.io/github/release/nightnoryu/pilate.svg)](https://github.com/nightnoryu/pilate/releases)

Configuration files for my LAN infrastructure on Raspberry Pi.

## Components

- DNS: [Pi-hole](https://pi-hole.net)
- Git server: [Gitea](https://about.gitea.com/products/gitea)
  - with PostgreSQL as database backend
  - and an [act_runner](https://gitea.com/gitea/act_runner) worker for CI/CD via Gitea Actions
- Monitoring stack: [Grafana](https://grafana.com)
- Reverse proxy gateway: [Nginx](https://nginx.org)

## Installation

### Requirements

- Raspberry PI 5 (with 8GB+ RAM)
- Ubuntu (Server or Desktop)
- Docker and docker compose

### Bootstrapping

TODO
