# :strawberry: Pilate [![Github release](https://img.shields.io/github/release/nightnoryu/pilate.svg)](https://github.com/nightnoryu/pilate/releases)

Configuration files for my Raspberry Pi 5 hosted services.

## Components

- Git server: [Gitea](https://about.gitea.com/products/gitea)
  - with MySQL 8 as database backend
  - and an [act_runner](https://gitea.com/gitea/act_runner) worker for CI/CD via Gitea Actions
- Monitoring system: [Grafana](https://grafana.com)
- Reverse proxy gateway: [Nginx](https://nginx.org)

## Installation

### Requirements

- Raspberry PI 5 (with 8GB+ RAM)
- Ubuntu (Server or Desktop)
- Docker and docker compose

### Bootstrapping

TODO

## Managing

The whole system is be managed with a simple convenience script: `compose`. The first argument is the service directory (e.g. `gitea` or `gateway`) and the others are the usual `docker compose` arguments. For example:

```shell
# Start all the services
./compose gitea up -d
./compose grafana up -d
./compose gateway up -d

# Check the logs for gateway
./compose gateway logs gateway

# Check the statuses of gitea containers
./compose gitea ps
```
