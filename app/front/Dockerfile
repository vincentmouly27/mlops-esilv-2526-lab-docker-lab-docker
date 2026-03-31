# 1. On utilise Nginx (serveur web léger)
FROM nginx:alpine

# 2. On définit le dossier de travail pour Nginx
WORKDIR /usr/share/nginx/html

# 3. On copie le contenu du dossier front vers le dossier par défaut de Nginx
COPY . .

# 4. On expose le port 80 (port standard du web)
EXPOSE 80

# 5. Pas besoin de CMD complexe, Nginx démarre tout seul