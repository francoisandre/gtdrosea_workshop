# Ateliers ROSEA : Programme python

## Les bases python et numpy

### base du python
- les différents types d'objets
    * typage dynamique
    * list
    * tuple
    * fonction type
- les structures de contrôle
    * if then else
    * surtout boucle for par rapport à langages type fortran ou c
    * list intrprétée
- ecrire une fonction
- importer des modules, où les chercher
- la gestion des dates
- essayer de montrer comment interpréter les messages d'erreur?

### présentation de numpy
- differences avec le python standard
- l'objet array/ndarray
- déclaration des tailles des tableaux quasi-obligatoire

## Lire et ecrire des fichiers

### lecture écriture "classique"
- `with open(filename, 'rb') as f:`
- readlines()
- supprimer les caractères de changements de lignes

### lecture de fichiers colonnes (données 1d)
- utilisation de np.genfromtxt
- conversion de la colonne date à la volée
- association de plusieurs colonnes pour former la date
- peut-être premier exemple de tracé des données avec matplotlib

### exemple de lecture de données binaires avec fromfile
- prendre exemple de données IPRAL (mélange ASCII+binaire)
- données 2d
- exemple de fichiers binaire au format fortran?

### lecture/écriture de fichiers netCDF avec module netCDF4
- ouverture du fichier
    * voir la liste des variables (équivalent ncdump -h)
    * récupérer le contenu des variables et des attributs
- ecrire un fichier netCDF
    * créer les dimensions
    * ajouter des attributs globaux
    * créer les variables et y ajouter des valeurs et des attributs
- finir sur un exercice qui regroupe les compétences
    * lecture d'un fichier 1d texte
    * lecture de données 2d (binaire?)
    * écriture des données dans un fichier netCDF

### tracer des données avec matplotlib
- traçage de graphe 1d
- traçage de graphes 2d type lidar
- changer les couleurs et les types de lignes
- plusieurs graphe sur une même figure
- traçage sur carte avec basemap?

### créer un module
- regrouper l'ensemble de ce qui a été fait dans un module
- le faire uniquement en procédural = pas de création de classe
- montrer les bonnes pratiques pour le python 2
    * `from __future__`
    * docstring pour chaque fonction
    * `if __name__ == '__main__':`
    * argument d'entrée avec argparse?
- possibilité de commencer à montrer comment faire des tests unitaires et exécuter les tests avec __nosetests__ et activer le coverage
- parler de pep8 pour le contrôle de la syntaxe et __pylint__ pour évaluer son code

### documentation
- A partir du module montrer l'utilisation de sphinx pour le commenter
- configuration de sphinx/structure de la documentation
- commencer à écrire le code
- syntaxe à ajouter dans le module pour se faire comprendre de sphinx

