# Utilisez une image de base avec Node.js préinstallé
FROM node:14

# Définissez le répertoire de travail dans le conteneur
WORKDIR /app

# Copiez les fichiers package.json et package-lock.json pour installer les dépendances
COPY package*.json ./

# Installez les dépendances
RUN npm install

# Copiez les fichiers de l'application dans le conteneur
COPY . .

# Exposez le port sur lequel votre application écoute
EXPOSE 3001

# Commande pour démarrer l'application
CMD ["npm", "start"]
