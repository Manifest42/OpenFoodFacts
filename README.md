# OpenFoodFacts



## Contenu du repository
- Le script d'initialisation de la bdd dans database
- Le code de l'application dans utils et main.py
- La documentation dans le README.md
- Le fichier requirements.txt pour installer les librairies python

## Installation


- Pour installer l'application et la lancer, commencez par cloner le repo:
```bash
git clone https://github.com/Manifest42/OpenFoodFacts.git
```
    
- Installez virtualenv si ce n'est pas déja fait:
```bash
pip3 install virtualenv
```

- Créez un environnement virtuel:
```bash
virtualenv venv
```

- Activez cet environnement:
```bash
source venv/bin/activate
```

- Installez les requirements:
```bash
pip3 install -r requirements.txt
```

- Lancez le programme:
```bash
python3 main.py
```

## Fonctionnalités

#### Choisir entre chercher un produit ou voir les aliments substitués
    Le programme doit afficher les choix disponibles, quelle commande permet
    de faire son choix ( exemple: 0: chercher produit, 1: voir substituts ),
    et qu'on puisse envoyer notre choix a l'application.

    
#### Afficher les catégories et en choisir une
    Le programme doit aller chercher des catégories sur l'api OpenFoodFacts
    et les afficher avec la commande correspondante et permettre de rentrer
    dedans pour voir les produits disponibles
  
#### Afficher les produits et en choisir un
    Le programme doit aller chercher les produits contenus dans une catégorie
    donnée. Les afficher avec la commande correspondante et permettre de
    voir leurs infos et un substitut.

#### Voir les substituts
    Le programme doit aller chercher les substituts que l'utilisateur a
    sauvegardés en bdd et les afficher avec la commande correspondante pour accéder
    à leur details.
    
#### Communiquer avec la bdd
    Le programme aura une classe Database() qui se connectera a la base de
    données a son initialisation et qui contiendra des méthodes génériques
    pour communiquer avec la base de données.

#### Pouvoir modifier les valeurs importantes facilement
    Le programme inclura un fichier settings.py dans lequel on pourra modifier facilement
    les identifiants de connexion a la base de données et le nombre d'aliments et de produits
    à récupérer
