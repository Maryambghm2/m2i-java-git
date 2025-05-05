# Git 

## Commandes principales 

### Initialiser un répertoire de travail Git 

```bash
git init
```

### Visualiser les modification actuelles du dossier de travail

```bash
git status
```
### Ajouter un fichier /emplacement dans le repository

* Pour ajouter un emplacement à la staging area 
```bash
git add chemin/de/fichier
```

* Pour ajouter tous les fichiers de notre emplacement racine à la staging area
```bash
# Syntaxe classique
git add .

# Autres syntaxes 
git add --all
git add -A
```

### Enregistrer les changements dans le repository

```bash
git commit -m "Message du commit"
```

### Connexion ; Utiliser global si 1 seul user dans le pc sinon utiliser local si plusieurs user 

### Afficher le informations des commits

```bash
git log
```

### Pour passer d'une branche à l'autre 

* Syntaxe à l'ancienne
```bash
git checkout nom-de-la-branche
```
# Pour créer la branche en même temps que de naviguer dessus
```bash
git checkout -b nom-nouvelle-branche
```
# Syntaxe moderne
```bash
git switch nom-de-la-branche
```
# Pour créer la branche en même temps que de naviguer dessus
```bash
git switch -c nom-nouvelle-branche
```
#Annuler un changement après avoir commit 
```bash
git revert <id-commit>
```
# Comparer les changements entre commits : 
```bash
git diff <id-commit>
```
Pour comparant deux commis précédents
```bash
git diff <id-commit-A> <id-commit-B>
```

# Pour revenir en arrière dans les commits 

```bash
fit reset <id-commit>
```

# Si on veut retirer les changement 

```bash
fit reset <id-commit>
```

# Pour cloner un repos
```bash
git clone <url-repos>
```

# Si l'on veut également chooisir le nom du dossier ou va être cloner le repertoire
```bash
git clone <url> <nom-dossier>
```