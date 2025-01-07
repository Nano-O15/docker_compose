# Utiliser une image de base Node.js
FROM node AS build

# Définir le répertoire de travail
WORKDIR /usr/src/app

# Copier package.json dans le conteneur
COPY package.json ./

# Installer les dépendances Node.js
RUN npm install

# Copier le reste des fichiers de l'application dans le conteneur
COPY . .

# Exposer le port 8000 pour accéder à l'application
EXPOSE 8000

# Commande pour démarrer l'application
CMD [ "npm", "start" ]