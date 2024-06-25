# Utilisation d'une image Node.js avec Alpine Linux comme base
FROM node:lts-alpine

# Création du répertoire de travail
WORKDIR /app

# Copie du package.json et du package-lock.json pour installer les dépendances
COPY package.json ./

# Installation des dépendances
RUN npm install

# Copie du reste des fichiers de l'application
COPY . .

# Exposition du port sur lequel le serveur Express écoute
EXPOSE 5678

# Commande pour démarrer l'application
CMD ["npm", "start"]
