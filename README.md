# Sup de Vinci - Projet Containers

Ce projet consiste à créer une application appelée "Joke of the Day" qui se compose d'une API construite avec Rust et d'une application front-end développée avec Next.js. 

## Prérequis

Avant de commencer, assurez-vous d'avoir installé Docker et Docker Compose sur votre machine.

- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)

## Lancement des Conteneurs

Pour démarrer les conteneurs pour l'application API et le front-end, suivez ces étapes :

1. **Clonez le dépôt** :

   ```bash
   git clone https://github.com/votre-utilisateur/sdv-m1do-containers-project.git
   cd sdv-m1do-containers-project

2. **Construisez et lancez les conteneurs** :

  Dans le répertoire racine de votre projet, exécutez la commande suivante pour démarrer Docker Compose :

    ```bash
    docker-compose up --build
  
  Cette commande va construire les images Docker pour l'API et le front-end, puis démarrer les conteneurs.

3. **Accéder à l'application** :

   Une fois les conteneurs lancés, vous pouvez accéder à l'application front-end à l'adresse suivante :

   http://localhost:3000

## Dans le cas d'une MAJ du code :

Lorsqu'un changement est effectué dans le code source, vous devez relancer Docker Compose pour appliquer les modifications. Voici comment procéder :

1. **Arrêt des conteneurs** :

Vous pouvez le faire en utilisant Ctrl + C dans le terminal où Docker Compose est en cours d'exécution.

2. **Relancez Docker Compose** :

   Exécutez la même commande qu'auparavant pour reconstruire et relancer les conteneurs :

     ```bash
    docker-compose up --build

## Déploiement des Images Docker :

Lors d'un push vers le repository git distant sur la branche MAIN l'image est automatiquement créé vous les retrouverez sur le repository suivant :

https://hub.docker.com/repository/docker/gyosei/container-joke
