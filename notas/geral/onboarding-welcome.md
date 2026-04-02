# onboarding-welcome

_Exportado em 02/04/2026_

 Docker/Containers
Vamos aproveitar o paradoxo: usar containers para aprender Linux, sendo que containers são baseados em Linux! Mente explodida? 🤯

Passo 1: Instalar Docker
Windows/macOS: Docker Desktop
Linux:
# Ubuntu
sudo apt install docker.io
# RHEL/CentOS
sudo dnf install docker

Passo 2: Rodar Containers de Diferentes Distros
Ubuntu:
docker run -it --name ubuntu-lab ubuntu:latest bash

Alpine:
docker run -it --name alpine-lab alpine:latest sh

Rocky Linux:
docker run -it --name rocky-lab rockylinux:latest bash

Debian:
docker run -it --name debian-lab debian:latest bash

Esta opção é a mais leve e permite experimentar várias distros rapidamente, mas tem limitações para aprender sobre serviços, systemd e outras partes do sistema.

