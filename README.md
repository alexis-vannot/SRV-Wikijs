# SRV-Wikijs

## Lancement du conteneur

```shell
docker compose up --build -d
```

## Arrêt du conteneur

```shell
docker compose down --remove-orphans
```

## Rentrer dans le conteneur

```shell
docker exec -it wikijs bash
docker exec -it postgresql-wikijs bash
```

## Informations

### Wikijs

- Certaines variables d'environement utilisées sont stockées dans le fichier `./.secrets/wikijs.env` sur l'hôte.

### Postgresql

- La seule variable d'environement utilisée est stockée dans un "secrets" dans le dossier `./.secrets/` sur l'hôte.

- Les données persistantes sont dans le dossier `./postgresql_data` sur l'hôte.
