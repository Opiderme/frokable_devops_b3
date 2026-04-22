# Image de base
FROM python:3.12-slim

# Dossier de travail dans le conteneur
WORKDIR /app

# Installation des dépendances
COPY requirements.txt .
RUN pip install -r requirements.txt

# Copie du code
COPY . .

# Export du port
EXPOSE 8000

# Commande de démarrage
CMD uvicorn main:app --host 0.0.0.0 --port 8000
