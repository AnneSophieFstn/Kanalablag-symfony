# KANALABLAG - Symphony 6

## Description

Une application sécurisée sur les blagues.

## Fonctionnalités

- En tant qu'utilisateur, je doit pouvoir me connecter à une interface sécurisée.
- En tant qu'utilisateur **connecté**, je doit pouvoir créer | modifier | supprimer une catégorie.
- En tant qu'utilisateur **connecté**, je doit pouvoir créer | modifier | supprimer une blague.
- En tant qu'utilisateur **non connecté**, je doit pouvoir voir la liste des blagues.
- En tant qu'utilisateur **non connecté**, je doit pouvoir voir la liste des catégories.

## Technologies

**Backend:**

- Symfony

**Frontend:**

- Twig, Html, Css

## Installer et exécuter le projet

1. Renommer le fichier `.env.example` en `.env`

Si vous utilisez mysql à la ligne 27

- Entrer les différentes informations en fonction de vos données à vous:

`DATABASE_URL="mysql://NAME_HOST:@127.0.0.1:3306/NAME_DATABASE?charset=utf8mb4"`

- Si vous n'utilisez pas mysql, n'oubliez pas de commenter la ligne et d'utiliser celle qui convient à votre bdd.

2. Une fois que l'étape 1 est faites, ouvrez le terminal et lancer les commandes suivantes

- `symfony console make:migrations`
- `symfony console doctrine:migration:migrate`

3. Lancer votre server

- `symfony serve`

4. Rendez-vous sur le lien de votre server.
