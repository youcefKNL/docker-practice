# Utilisation de l'image Node.js comme base
FROM node:20.15.0

# Définition du répertoire de travail dans le conteneur
WORKDIR /app

# Copie des fichiers du frontend dans le conteneur
COPY ./ /app

# Installation de http-server globalement (si non installé)
RUN npm install -g http-server

# Exposition du port 80 pour http-server
EXPOSE 80

# Commande pour démarrer http-server
CMD ["http-server", "-p", "80"]
