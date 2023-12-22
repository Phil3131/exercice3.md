1- Donne une ligne de commande bash qui permet de lister la liste des utilisateurs d'un système Linux

    les Utilisateurs sont dans le fichier /etc/passwd on peut faire une recherche avec Grep afin de trouver l'utilisateur souhaité.


2- Quelle commande bash permet de changer les droits du fichier myfile en rwxr—r-- ?

    Commande CHMOD . Plus en détail   ->   chmod 744 myfile


3- Quelle est la différence entre une variable d'environnement et une variable locale dans un script Bash, et comment pouvez-vous les définir et les utiliser ?

4- Expliquez comment fonctionne la structure de contrôle "if" dans Bash. Donnez un exemple concret de son utilisation pour prendre une décision basée sur une condition dans un script Bash.

    if est une condition "si" a placer entre crochet [] suivi de else que l'on pourrait traduire par "alors" on peut rajouter une autre condition avec ELIF (else if) . On termine par fi (if a l'envers) 

    if [ condition ]; then
    # notre condition
    else
    # la condition est fausse
    fi

    plus en detail 

    Structure conditionnelle if
    if condition
    then
	  instructions
    elif conditions2		(optionnel)
    then
	  instructions
    else					(optionnel)
	instructions
fi

5- Donne la(les) ligne(s) de commande(s) bash pour afficher le texte suivant :
Malgré le prix élevé de 100$, il a dit "Bonjour !" au vendeur :
- "Bonjour est-ce que ce clavier fonctionne bien ?"
- "Evidemment ! On peut tout écrire avec, que ce soit des pipe | ou bien des backslash \\ !"
- "Même des tildes ~ ?"
- "Evidemment !"

      echo "Malgré le prix élevé de 100\$, il a dit \"Bonjour !\" au vendeur :"
      echo "- \"Bonjour est-ce que ce clavier fonctionne bien ?\""
      echo "- \"Evidemment ! On peut tout écrire avec, que ce soit des pipe | ou bien des backslash \\\\ !\""
      echo "- \"Même des tildes ~ ?\""
      echo "- \"Evidemment !\""

      on utilise des \ pour "echapper" les symboles ! ? " etc etc afin qu'ils soient lu dans la phrase entiere. 


6- La commande jobs -l donne le résultat ci-dessous :
wilder@Ubuntu:~$ jobs -l
[1]  37970 En cours d'exécution   gedit &
[2]  37971 En cours d'exécution   xeyes &
[3]- 37972 En cours d'exécution   sleep
Quelle commande te permet de mettre en avant le processus gedit ?

    il s'agit de la commande fg 




7- Quels matériels réseaux sont sur la couche 2 et la couche 3 du modèle OSI ? Donne leurs spécificités.

    Couche 2 du Modele OSI - Liaison de données
    Switch -> Permet de relier plusieurs segments d'un reseau infomatique . ils trient le trafic en fonction des adresses MAC (adresse physique) Une sorte de       
    "multiprise"   reseau. 

    Couche 3 du modéle OSI - Reseau 
    Routeur -> Assure le routage et l’interconnexion de réseaux hétérogènes. Peut etre parametrable. 
   
8-  Quels sont les équivalent PowerShell des commandes bash cd, cp, mkdir, ls.

    cd (Change Directory) :

    Bash : cd chemin/vers/le/dossier
    PowerShell : Set-Location chemin/vers/le/dossier
    cp (Copy) :

    Bash : cp source destination
    PowerShell : Copy-Item source destination
    mkdir (Make Directory) :

    Bash : mkdir nom_du_dossier
    PowerShell : New-Item -ItemType Directory -Name nom_du_dossier
    ls (List) :

    Bash : ls
    PowerShell : Get-ChildItem

    
10. Dans la trame ethernet, qu'est-ce que le payload ?
11. Pourquoi les classes IP sont remplacées par le CIDR ?
