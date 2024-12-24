# Utiliser l'image de base Ubuntu 22.04
FROM ubuntu:22.04

# Définir les variables d'environnement
ENV DEBIAN_FRONTEND=noninteractive

# Mettre à jour les paquets et installer les dépendances nécessaires
RUN apt-get update && apt-get upgrade -y && \
    apt-get install -y \
    python3 \
    python3-pip \
    python3-dev \
    build-essential \
    curl \
    git \
    vim \
    && apt-get clean

# Installer numpy et autres paquets Python nécessaires
RUN pip3 install --upgrade pip && \
    pip3 install numpy

# Définir la commande par défaut pour démarrer le conteneur
CMD ["bash"]