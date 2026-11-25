# TP4 - Docker et Docker Compose

## Objectif
Conteneuriser une application React et une API Express avec Docker Compose.

## Architecture
- Client : application React compilee puis servie sur le port 3000.
- Serveur : API Express sur le port 9000.
- MongoDB : base de donnees MongoDB sur le reseau Docker mern-network.

## Construction et lancement
Depuis la racine du projet, executer :

```cmd
docker compose up --build
```

## Verification
- Client : http://localhost:3000
- API : http://localhost:9000/api/health
- L'API doit retourner le message API is running.

## Arret
```cmd
docker compose down
```

## Captures
- captures/conteneurs.png : conteneurs Docker actifs.
- captures/images.png : images Docker construites.

## Variable d'environnement
Le service serveur recoit MONGO_URI depuis Docker Compose.
Le code actuel du serveur ne se connecte pas encore a MongoDB.
