# php 7.4 / mysql8 / nginx / projet Symfony 5.x

## Installation de l'environnement avec Docker

Cloner le repository et executer `docker compose up -d --build`

## Création d'un projet Symfony

Accéder au conteneur php : `docker exec -it php74-container bash`
Créer du projet : `composer create-project symfony/skeleton .`
Tester l'installation : `localhost:8080`


