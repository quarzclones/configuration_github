Procédure d'ajout d'utilisateur
===============================

-------------------------------

1 - Ajouter un utilisateur au repository
----------------------------------------

* Aller sur le repository en question
* Cliquer sur "settings"
* Cliquer sur "Manage access"
* Cliquer sur "Invite a collaborator"
* Ecrire l'email de l'utilisateur à inviter et cliquer sur l'utilisateur dans le déroulant

2 - Ajouter une clef SSH sur son compte github
----------------------------------------------

Cette procédure vise à permettre les commandes "git" en relation avec les repository de github.
Avec l'invitation des utilisateurs au repository, ceci simplifie et sécurise le repository en question

* Cliquer sur son image de profil en haut à droite puis sur "settings"
* Cliquer sur "SSH and GPG Keys"
    * C'est ici que nous allons renseigner le nom et la clé SSH de notre key

* Pour Mac et Linux, ouvrez le Terminal / Pour Windows, ouvrez Git Bash
* Entrez la commande " ssh-keygen -t ed25519 -C "your_email@example.com" "
* Passez toute les étapes, elles importent peux
* Entrez la commande " cd ~/.ssh " puis " ls "
* Dans la liste, il devrait y avoir un fichier nommé " id_ed25519.pub "
* Entrez la commande " cat id_ed25519.pub "
* Le contenu devrait s'afficher, copier à partir de (en le copiant aussi) "ssh-ed25519" jusqu'à la fin de la clef (ne pas copier le contenu qui suit, en soit l'email s'il est affiché)
    * Example : ssh-ed25519 A34546YTRE5TERT5ERT4ETFE43ZEDR3ESFC4Z3RCE4TCG4T4V
* Sur Github, cliquez sur " New SSH key ", Donnez lui un nom puis copiez la clef à l'endroit prévu à cette effet
* Cliquez sur " Add SSH key "

Fichier édité par : Guillaume " Levios " Douchement