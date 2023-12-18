# Symfony Projet HB Shop

Ce projet est un système de gestion de liste de produits.

### Techno

- Symfony - Framework d'application web en PHP
- Bootstrap - outils pour le développement avec HTML, CSS et JS
- Sonata Admin - fournit des fonctionnalités d'administration (Plus complexe que EasyAdmin... ;))
- Knp Paginator - paginateur Symfony

### Exigences

- PHP 7.1.3 ATTENTION PAS 8.2 ! Sinon il y aura des problèmes avec les dépendances
- MySQL
- Composer

### Installation

Configuration de la base de donnée :

- A la racine du projet créer un fichier .env
- Remplir le fichier avec l'url de votre base de donnée

Installez les dépendances

```sh
$ composer install
```

Configurez la base de données et créez le schéma à partir des migrations

```sh
$ php bin/console d:d:c
$ php bin/console d:m:m
```

Chargez les fixtures

```sh
$ php bin/console d:f:l
```

Lancez le serveur

```sh
$ symfony serve --no-tls
```

### Utilisation

- Allez sur l'équivalent de ce lien en fonction de votre machine http://127.0.0.1:8080/admin/login
- Connectez-vous avec le nom d'utilisateur et le mot de passe (identifiants de connexion ci-dessous)
- Ajoutez des catégories et des produits
- Allez sur la page principale pour voir une liste de catégories
- Cliquez sur un élément de la liste des catégories pour voir une liste de produits

### Connection

Nom d'utilisateur | Mot de passe | Rôles
--- | --- | ---
root | root | ROLE_ADMIN
admin | admin | ROLE_ADMIN
