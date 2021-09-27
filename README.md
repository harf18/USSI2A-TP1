# TP1 : GIT & GitHub Classroom

### Objectif

Se familiariser avec GIT / Github Classroom / Pull request

### Prérequis

- Ouvrir Git Bash, aller dans le dossier de votre choix et créer un dossier USSI2A. Par exemple :  

```
$ cd  
$ cd Documents  
$ mkdir USSI2A
$ cd USSI2A
```
- Sur github, sur la page d'accueil du projet, cliquer sur le bouton vert "code" et copier le l'url ```https://github.com/Le-Cnam/tp1...```
- Cloner le projet GITHUB sur votre poste :  

```
$ git clone <COLLER L'URL COPIEE CI DESSUS>  
```

- Saisir vos identifiants github  

- Git va récupérer le projet. Visualiser le dossier, puis aller dans le dossier :

```
$ ls -ltr
$ cd tp1-XXXXXX (ou XXXXX = votre username)
```

- Vous remarquez **(master)** en fin de ligne : vous êtes sur la branche master  

- Créer une nouvelle branche, puis aller sur la branche :  

```
$ git branch prenomNom
$ git checkout prenomNom
```

- Vous remarquez **(prenomNom)** en fin de ligne : vous êtes sur la branche prenomNom.  Git change le contenu de votre repertoire en fonction de la branche sur laquelle vous êtes. La branche master ne sera pas impactée par vos modifications.

  

### IntelliJ

- Ouvrez IntelliJ
- Ouvrir le projet USSI2A-TP1 :
	- Sur l'écran d'accueil d'IntelliJ, cliquer sur **New Project**
	- Selectionner **Java** dans la liste de gauche et **17** dans **Project SDK** puis **Next**
	- Ne rien cocher puis **Next**
	- Cliquer sur les **...** de **Project location** puis selectionner le dossier du projet et cliquer sur **OK**
	- Cliquer sur **Finish**
	- Le projet s'ouvre



### Votre 1er programme Java 17

- Dans le navigateur de projet a gauche, developper **tp1-XXXXXX > src** en cliquant sur la fleche devant src
- Double cliquer sur HelloWorld : dans la fenêtre principale d'IntelliJ, la classe HelloWorld s'ouvre, ajouter le contenu nécessaire pour créer un Hello World.
- Pour l'excuter, cliquer droit sur **main** et cliquer sur "Run HelloWorld.main"
- Hello World doit s'écrire dans la fenêtre en bas d'IntelliJ



### Envoyez votre travail

- Dans GIT bash, ajouter votre travail dans la "zone prêt à commiter" :

```
$ git add .
```

- Commitez votre travail (faire un commit = enregister votre code dans l'historique des modifications) : 

```
$ git commit -m "<Un message de commit comprehensible et qui décrit bien votre travail>"
```

- Envoyer votre branch nomPrenom sur le serveur

```
$ git push origin prenomNom
```

- Aller sur GitHub et Cliquer sur **New Pull Request**, base = *master*, compare = votre branche *prenomNom*, puis cliquer sur **Create Pull Request**
