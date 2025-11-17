# Utiliser l'image officielle Node.js
FROM node:latest

# Définir le répertoire de travail
WORKDIR /app

# Copier les fichiers package.json et package-lock.json
COPY package.json ./

# Installer les dépendances
RUN npm install

# Copier le reste des fichiers de l'application
COPY . .

# Compiler l'application pour la production
RUN npm run build

# Exposer le port 3000
EXPOSE 3000

# Démarrer l'application en mode production
CMD ["npm", "start"]