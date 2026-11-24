# Image Node.js
FROM node:24-alpine

# Dossier de travail
WORKDIR /app

# Copier les fichiers package
COPY package*.json ./

# Installer les dépendances
RUN npm install

# Copier le projet
COPY . .

# Exposer le port Vite
EXPOSE 3000

# Lancer React
CMD ["npm", "run", "dev", "--", "--host", "0.0.0.0"]