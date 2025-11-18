Examen Pratique
I.	Initialiser un dépôt Git local :
1. Créez un nouveau répertoire prenom-nom-netmiko pour votre projet.
$ mkdir arij-belaid-netmiko
$ cd  arij-belaid-netmiko

3. Initialisez un dépôt Git dans ce répertoire.
$ git init


II. Ajouter et commiter des fichiers
1.	Créez un fichier README.md et ajoutez-y le titre : Mon Projet Netmiko
$ touch README.md
$ vim README.md

2.	Ajoutez ce fichier à l'index et commitez-le en utilisant le message "Ajout  du fichier README".
$ git add -A
$ git commit -m "Ajout du fichier README"

3. Créez un fichier main.py et ajoutez-y un simple script Python : print("Hello, Git!")
$ touch main.py
$ vim main.py

3.	Ajoutez et commitez ce fichier en utilisant le message "Ajout du script Python principal".
$ git add -A
$ git commit -m "Ajout du script Python principal"


II.	Créer et fusionner des branches
1.	Créez une nouvelle branche feature/netmiko pour ajouter une fonctionnalité.
$ git branch feature/netmiko

2. Modifiez main.py pour inclure une fonction acces_netmiko qui utilise la bibliothèque
netmiko pour effectuer les opérations suivantes sur un routeur Cisco C8000V :
$ vim main.py

4. Ajoutez et commitez ces modifications avec le message "Ajout de la fonction
acces_netmiko".
$ git add -A
$ git commit -m "Ajout de la fonction acces_netmiko"

5.	Revenez à la branche principale (main).
$ git checkout master

III.	Travailler avec un dépôt distant sur GitHub
2. Ajoutez ce dépôt GitHub comme dépôt distant.
git remote add origin https://github.com/votre-username/prenom-nom-netmiko.git

3.Poussez vos commits locaux vers GitHub.
git push -u origin main

6.	Sur votre machine locale, récupérez cette nouvelle branche.
$ git fetch origin
$ git checkout -b feature/salut origin/feature/salut


7.	Modifiez main.py pour ajouter une fonction qui dit salut.
$vim main.py

9.	Ajoutez et commitez ces modifications avec le message "Ajout de la fonction dire_salut".
$ git add main.py
$ git commit -m "Ajout de la fonction dire_salut"

9.	Poussez cette branche vers GitHub.
$ git push origin feature/salut

12. Revenez à la branche main locale et récupérez les dernières modifications
$ git pull origin main
$ git branch -d feature/salut




