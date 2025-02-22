# Projet Git sous Linux

Auteur:
Adabire 
# Description du projet

Ce projet vise à illustrer l'utilisation des commandes Git fondamentales sur un système Linux. En créant un script simple et en explorant diverses fonctionnalités Git (branches, tags, gestion des conflits, etc.), il permet de mieux comprendre la gestion de versions et le suivi des modifications dans un projet.

# Objectifs du projet

Ce projet illustre l'utilisation des commandes Git essentielles sous Linux. À travers la création d’un script simple et l’exploration de diverses fonctionnalités Git (comme la gestion des branches, l’utilisation des tags et la résolution de conflits), il permet de se familiariser avec le contrôle de version et le suivi des modifications dans un projet.
# Copier le code
sudo apt update
sudo apt install git
Configuration :
bash
# Copier le code
git config --global user.name "Adabire"
git config --global user.email "exemple@domaine.com"
Initialisation du projet
Créer un dossier de travail, work, et un sous-dossier, hello.

bash
# Copier le code
mkdir -p work/hello
cd work/hello
Initialiser un dépôt Git :

bash
# Copier le code
git init
Création et gestion des fichiers
Créer un fichier hello.sh :
bash
# Copier le code
echo 'echo "Hello, World"' > hello.sh
Ajouter et valider le fichier dans le dépôt :
bash
# Copier le code
git add hello.sh
git commit -m "Initial commit with Hello World script"
Création et gestion de branches
Créer une branche greet pour ajouter une nouvelle fonctionnalité :
bash
# Copier le code
git checkout -b greet
Modifier hello.sh pour inclure une fonction de salutation personnalisée et ajouter le fichier dans le suivi Git :
bash
# Copier le code
echo 'echo "Hello, $1"' > hello.sh
git add hello.sh
git commit -m "Add greeting with parameter support"
Fusion et gestion des conflits
Fusionner la branche greet dans main :
bash
# Copier le code
git checkout main
git merge greet
Création de tags
Marquer une version stable du projet :
bash
# Copier le code
git tag v1 :git tag est utile pour marquer des étapes clés du projet et suivre les différentes versions.
Publier le projet sur GitHub
Créer un dépôt sur GitHub nommé hello.
Lier le dépôt GitHub au projet local :
bash
# Copier le code
git remote add origin https://github.com/username/hello.git
Pousser les modifications vers GitHub :
bash
# Copier le code
git push -u origin Master
Lien vers le dépôt GitHub
Consulter le dépôt GitHub (Remplace username par ton nom d’utilisateur GitHub)

Explications additionnelles
Branches : Utilisées pour développer des fonctionnalités en parallèle sans affecter la branche principale.
Tags : Créés pour marquer des versions spécifiques du projet, permettant de revenir facilement à une version stable.
Historique des commits
Pour consulter l'historique des commits, utiliser :

bash
# Copier le code
git log --oneline
License
Ce projet est sous licence libre 

Ce README.md décrit les étapes principales du projet, les commandes utilisées et les explications essentielles. Tu pourras l’ajouter à ton projet avec les commandes suivantes :

bash
Copier le code
git add README.md
git commit -m "Add README.md with project documentation"
git push
Ainsi, ton projet sera bien documenté et prêt pour l’évaluation sur GitHub.
