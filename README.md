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

- Cloner le projet GITHUB sur votre poste :  

```
$ git clone https://github.com/Le-Cnam/tp1-username.git  
```

- Saisir vos identifiants github  

- Git va récupérer le projet. Visualiser le dossier, puis aller dans le dossier :

```
$ ls -ltr
$ cd tp1-username
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
	- Sur l'écran d'accueil d'IntelliJ, cliquer sur **Import Project**
	- Selectionner le dossier du projet
	- Selectionner **Create project from existing sources**
	- Conserver les informations (*Nom, Location, Format*)
	- IntelliJ détecte que c'est un projet Java
	- Aucune bibliothèque n'est integtée au projet
	- IntelliJ créé un modules USSI21-TP1
	- Choisir JDK17, s'il n'est pas dans la liste, cliquer sur le <span style="color:green">**+**</span> et selectionner le dossier du JDK 17
	- Aucun Framework n'est detecté
	- Aller dans File > Project Structure et Choisir 17 dans **Project language level**



### Votre 1er programme Java 17

- Dans le navigateur de projet, developper USSI2A-TP1 > src 
- Double cliquer sur HelloWorld : dans la fenêtre principale d'IntelliJ, la classe HelloWorld s'ouvre, ajouter le contenu nécessaire pour créer un Hello World.
- Pour l'excuter, cliquer droit sur **main** et cliquer sur "Run HelloWorld.main"
- Hello World doit s'écrire dans la fenêtre en bas d'IntelliJ



### Envoyez votre travail

- Dans GIT bash, ajouter votre travail dans la "zone prêt à commiter"

```
$ git add .
```

- Commitez votre travail (faire un commit = enregister votre code dans l'historique des modifications)

```
$ git commit -m "Mon travail pour ce TP1"
```

- Envoyer votre branch nomPrenom sur le serveur

```
$ git push origin prenomNom
```

- Aller sur GitHub et Cliquer sur **New Pull Request**, base = *master*, compare = votre branche *prenomNom*, puis cliquer sur **Create Pull Request**
