# Utilisation de la dernière image Node.js officielle en tant que base
FROM node:latest

# Création d'un répertoire de travail dans le conteneur
WORKDIR /app

# Copie du fichier package.json et package-lock.json (si présent) dans le conteneur
COPY package*.json ./

# Installation les dépendances du projet
RUN npm install

# Copie tous les fichiers source dans le conteneur
COPY . .

# Exposition du port sur lequel l'application Vue.js s'exécutera (par défaut : 8080)
EXPOSE 8080

# Commande pour exécuter l'application Vue.js en mode développement
CMD ["npm", "run", "serve"]