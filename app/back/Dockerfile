# 1. Image de base avec Python
FROM python:3.9-slim

# 2. On définit le dossier de travail dans le conteneur
WORKDIR /app

# 3. On copie le fichier des dépendances d'abord (optimisation du cache)
COPY requirements.txt .

# 4. On installe les bibliothèques (pip install)
RUN pip install --no-cache-dir -r requirements.txt

# 5. On copie tout le code du dossier back actuel vers /app
COPY . .

# 6. On expose le port 5000 (celui utilisé par Flask par défaut)
EXPOSE 5000

# 7. La commande pour démarrer l'application
CMD ["python3", "-m", "flask", "run", "--host=0.0.0.0"]