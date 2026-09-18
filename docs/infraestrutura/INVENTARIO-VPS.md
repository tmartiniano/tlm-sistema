# Inventário inicial da VPS

## Data

2026-09-18

## Sistema

- Ubuntu 24.04.5 LTS
- Kernel 6.8.0-138-generic
- Arquitetura amd64
- Virtualização KVM

## Recursos

- 4 vCPUs AMD EPYC
- 7,8 GiB de RAM
- 75 GB de disco
- Aproximadamente 66 GB livres
- Swap não configurada

## Docker

- Docker Engine 29.8.0
- Docker Compose 5.5.1
- Docker Swarm ativo
- Um nó
- Nó atual como manager e leader

## Serviços existentes

- easypanel
- easypanel-traefik

## Redes existentes

- easypanel: overlay
- ingress: overlay
- docker_gwbridge: bridge

## Portas identificadas

- 22: SSH
- 80: HTTP/Traefik
- 443: HTTPS/Traefik
- 3000: EasyPanel
- 2377, 7946 e 4789: Docker Swarm

## Volumes Docker

Nenhum volume Docker existente na auditoria inicial.

## Diretriz

O EasyPanel será o painel oficial para instalar e administrar os serviços do sistema.
