# onboarding-welcome

_Exportado em 02/04/2026_

1. Containers e Docker
Docker e praticamente todas as tecnologias de containerização dependem de recursos do kernel Linux:

# Ver namespaces em uso por um container
sudo lsns | grep nome_do_container

# Ver cgroups (control groups) de um container
ls -la /sys/fs/cgroup/*/docker/

# Um container Docker simples
docker run -d --name webserver nginx:alpine

O Docker usa:
Namespaces: Isolamento de processos, rede, mount points
Cgroups: Limitação e controle de recursos (CPU, memória)
Overlayfs: Sistema de arquivos em camadas
Capabilities: Controle granular de privilégios

