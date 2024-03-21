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

Étape 1 : création d'un dépôt Git sur GitHub
Se connecter à votre compte GitHub.
Cliquez sur le bouton "+" dans le coin supérieur droit de la page et sélectionnez "New repository".
Remplissez les détails du nouveau dépôt (nom, description, visibilité, etc.).
Cliquez sur "Create repository" pour créer le dépôt.

Étape 2 : Configuration du projet Flask
Créez un nouveau répertoire sur votre machine sur virtuel studio code pour le projet Flask.
Placez les fichiers app.py, test_app.py, et requirements.txt dans ce répertoire

Installez les dépendances :
pip install -r requirements.txt

Étape 3 : création d'une Azure Web App
Connectez-vous au portail Azure.
Cliquez sur "Create a resource" dans le coin supérieur gauche.
Cliquer sur crée web app
Remplir le nom
Exécution stack : python 3.10
Laisser tout par default 
Sauf au niveau de deployment : Basic Authentication : Enable. /!\
Il faut télécharger le profile azure pour cela cliquer sur "Download azure profile"

Étape 4 : création de la pipeline CI/CD sur GitHub Actions
Allez dans la menue action 
Rechercher python web app azure 
Puis cliquer sur configuré
Il faut maintenant changer le nom dans le code et le langage mettre en python3.10

Étape 5 : créez une action secret.
Dans le sitting, action et variable
Dans l'action, cliquer sur "new secret" nommé le fichier au même nom que dans le fichier yml
Puis coller le fichier que nous avons télécharger précédemment "azure profile"
Puis sauvegarder

Étape 6 : exécuter le CI/CD
Allez dans le menu action, on voit qu'une action est en train de se faire
Attendre qu'elle finisse puis va sur la page web azure.

Étape 7 : Changer le code de app.py
Change le code pour afficher un autre texte. 
Puis sauvegarder 
Dans la menue action, il va avoir une action qui se fait automatiquement. 
Puis rafraîchir la page 

FIN
