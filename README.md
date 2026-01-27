# travail-de-SE-GRP-10-SE-2026

# INSTALLATION ET CONFIGURATION DE KUBERNETES (K8s) SOUS UBUNTU 

L’objectif de ce rapport est de présenter les différentes étapes nécessaires à l’installation et à la configuration de Kubernetes sous Ubuntu, tout en expliquant les concepts essentiels liés à son fonctionnement en utilisant Minikube.

# Objectifs

- compredre la structure de K8s
- installer Docker
- installer Kubectl 
- installer et configurer Minikube

# Environnement

- VirtualBox Ubuntu 22.04
- Docker
- Minikube

# Introduction 

Kubernetes est un orchestrateur es conteneurs cree par Google. Ce document presente son installation locale avec Minikube.



## Auteurs

- [JOSUE PALANA ERNGER](https://github.com/PALANA1234/travail-de-SE-GRP-10-SE-2026)
- [SEMBALA POLOTO KARIM](https://github.com/PALANA1234/travail-de-SE-GRP-10-SE-2026)
- [TENGE-TENGE MUZINGA PRÉCIEUX](https://github.com/PALANA1234/travail-de-SE-GRP-10-SE-2026)
- [MANITU LANDA LANDRY](https://github.com/PALANA1234/travail-de-SE-GRP-10-SE-2026)
- [NZUZI NTEDIKA ESPERAND](https://github.com/PALANA1234/travail-de-SE-GRP-10-SE-2026)
- [MANUELLA MULUBA GABRIELA](https://github.com/PALANA1234/travail-de-SE-GRP-10-SE-2026)
- [MUDIA KIMPANI WILLY](https://github.com/PALANA1234/travail-de-SE-GRP-10-SE-2026)
- [LIZINATA KONGO DIEU-MERCI](https://github.com/PALANA1234/travail-de-SE-GRP-10-SE-2026)
- [KABAMBA TSHIDIUPUILA JOSEPH](https://github.com/PALANA1234/travail-de-SE-GRP-10-SE-2026)
- [GBOZE KAZONGO ELDEN](https://github.com/PALANA1234/travail-de-SE-GRP-10-SE-2026)




## Mise à jour du système

Mettre a jour le systeme pour eviter des erreurs 

```bash
sudo apt update 
sudo apt upgrade -y

```
## Installation de Docker
```bash
Sudo apt install Docker.io –y
Docker --version 
Sudo usermod –Ag docker $USER (autoriser ton utilisateur à utiliser Docker)

```

## Installation de Minikube
 
```bash
Curl –LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64

Sudo install minikube-linux-amd64   /usr/local/bin/minikube

Minikube version

```
## Installer Kubectl (Outil Kubernetes) 

```bash
Curl –LO “https://dl.k8s.io/release/$(curl -L -S https:// dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl”

Sudo install kebectl   /usr/local/bin/kubectl 

Kubectl version --client

```

## Démarrage et vérification du fonctionnement 

```bash
Minikube start --driver=docker

Kubectl get nodes 

Kubectl get pods -A

```
    
