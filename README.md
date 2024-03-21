# Projet CI/CD avec Flask et Azure Web App

## Description
Ce projet est un prototype réalisé dans le cadre de l'implémentation d'une pipeline de CI/CD pour une application Flask déployée sur Azure Web App.

## Fonctionnalités du projet
- Utilisation d'un dépôt Git sur GitHub.
- Mise en place de tests unitaires.
- Configuration d'une pipeline CI/CD avec GitHub Actions.
- Déploiement automatisé sur Azure Web App.

## Étapes clés du projet
1. **Création du dépôt Git :** Le dépôt a été créé sur GitHub pour héberger le code source du projet.
2. **Développement de l'application :** Le projet Flask a été développé en suivant les bonnes pratiques de développement logiciel.
3. **Création de l'Azure Web App :** Une Web App a été créée sur Azure pour déployer l'application.
4. **Récupération du profil Azure :** Le profil de publication a été récupéré depuis Azure et ajouté comme secret dans le dépôt GitHub.
5. **Configuration de la pipeline CI/CD :** Une pipeline CI/CD a été configurée avec GitHub Actions pour automatiser le build, les tests et le déploiement.
6. **Tests de la pipeline :** La pipeline a été testée en effectuant des changements de code dans le dépôt Git.

## Guide d'exécution du projet
### Prérequis
- Python 3.10 installé localement
- Un compte GitHub
- Un compte Azure

Étape 1 : Création d'un dépôt Git sur GitHub
Ce connectez à votre compte GitHub.
Cliquez sur le bouton "+" dans le coin supérieur droit de la page et sélectionnez "New repository".
Remplissez les détails du nouveau dépôt (nom, description, visibilité, etc.).
Cliquez sur "Create repository" pour créer le dépôt.

Étape 2 : Configuration du projet Flask
Créez un nouveau répertoire sur votre machine sur virtual studio code pour le projet Flask.
Placez les fichiers app.py, test_app.py, et requirements.txt dans ce répertoire

Installez les dépendances :
pip install -r requirements.txt

Étape 3 : Création d'une Azure Web App
Connectez-vous au portail Azure.
Cliquez sur "Create a resource" dans le coin supérieur gauche.
cliquer sur crée web app
remplir le nom
execution stack : python 3.10
laisser tout par default 
sauf au niveau de deployment : Basic Authentication : Enable. /!\
il faut télécharge le profile azure pour cela cliquer sur "Download azure profile"

Étape 4 : Création de la pipeline CI/CD sur GitHub Actions
allez dans le menu action 
rechercher python web app azure 
puis cliquer sur configuré
il faut maintenent changer le nom dans le code et le langage mettre en python3.10

Etape 5 : 




