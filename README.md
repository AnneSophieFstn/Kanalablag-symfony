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

## Pré-installation

1. Scoop (Package manager pour Windows)  
   [https://scoop.sh/](https://scoop.sh/)

2. php 8.1  
   [https://windows.php.net/downloads/releases/php-8.1.12-nts-Win32-vs16-x64.zip](https://windows.php.net/downloads/releases/php-8.1.12-nts-Win32-vs16-x64.zip)

Extraire sur le pc (par exemple dans mes documents)  
Ajouter à la variable d'environnement PATH le chemin vers le dossier extrait  
Pour vérifier que tout est ok, on peut ouvrir un terminal et tapper php -v pour voir la version de php utilisée par le système.

3. Symfony CLI  
   [https://symfony.com/download](https://symfony.com/download)

4. Composer  
   [https://getcomposer.org/Composer-Setup.exe](https://getcomposer.org/Composer-Setup.exe)

4bis. Installer git  
[https://github.com/git-for-windows/git/releases/download/v2.38.1.windows.1/Git-2.38.1-64-bit.exe](https://github.com/git-for-windows/git/releases/download/v2.38.1.windows.1/Git-2.38.1-64-bit.exe)

dans un terminal tapper :  
git config --global user.name "votre pseudo"  
git config --global user.email "[monadrresmail@gmail.com](https://mail.google.com/mail/?view=cm&fs=1&to=monadrresmail%40gmail.com&authuser=1)"

5. Créer un projet SYMFONY  
   symfony new --webapp bu

## Installer et exécuter le projet

1. Renommer le fichier `.env.example` en `.env`

Si vous utilisez mysql à la ligne 27

- Entrer les différentes informations en fonction de vos données à vous:

`DATABASE_URL="mysql://NAME_HOST:PASSWORD@127.0.0.1:3306/NAME_DATABASE?charset=utf8mb4"`

- Si vous n'utilisez pas mysql, n'oubliez pas de commenter la ligne et d'utiliser celle qui convient à votre bdd.

2. Une fois que l'étape 1 est faites, ouvrez le terminal et lancer les commandes suivantes

- `symfony console make:migrations`
- `symfony console doctrine:migration:migrate`

3. Lancer votre server

- `symfony serve`

4. Rendez-vous sur le lien de votre server.
