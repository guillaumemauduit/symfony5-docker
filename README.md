# php 7.4 / mysql8 / nginx / projet Symfony 5.x

## Installation de l'environnement avec Docker

- Cloner le repository et executer `docker compose up -d --build`.

## Création d'un projet Symfony

- Accéder au conteneur php : `docker exec -it php74-container bash`.
- Créer le projet : `composer create-project symfony/skeleton .`.
- Tester l'installation : `localhost:8080`.
- Installation de doctrine : `composer require doctrine`.

## Configuration mysql et création base de données
- Modifier le fichier .env de l'application : `DATABASE_URL="mysql://root:secret@mysql8-service:3306/symfony5-docker?serverVersion=8"`.
- Créer la base : `docker-compose run -rm php74-service php bin/console doctrine:database:create`.

