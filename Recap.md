# Formation Integra11y Recap

## **P1-J01**

### Git :
SCM (Source Code Manager), un gestionnaire de version qui permet de garder dans un historique les différentes étapes du développement.

### Github Pages : 
Permet d'ajouter des pages en markdown à notre projet. Github nous fournira une adresse internet afin qu'on puisse voir le résultat en ligne. Il nous propose plusieurs thèmes pour customiser la page.

### Configuration de Git en Local :
 Dans le termianl, avec la commande git config, on va pouvoir configurer certaines informations afin de signer correctements les commits.

On a <br/>
*ajouté le nom d'utilisateur* : ```git config --global user.name ."nom_user"``` <br/>*ajouté l'adresse email* : ```git config --global user.email "notre@email"```.

Pour vérifier que ces informations ont bien été enregistrées, on peut les lister dans le terminal : ```git config --global --list```.


### git clone : 
Cette commande permet de récupérer une copie d'un dépot distant sur notre machine. On peut ainsi travailler en local avec VSCode, ce qui est plus pratique que de travailler directement sur github.

### git pull : 
Avec cette commande, on va pouvoir récupérer le projet distant mis à jour dans notre dépot local.

### git add : 
Dans VSCode, on peut ajouter une nouvelle version d'un fichier à la zone de surveillance en cliquant sur le bouton + dans la section "Controle de code source".

### git commit : 
Avec cette commande, on enregistre dans l'historique une nouvelle version de notre application. Dans VSCode, dans la section "Controle de code source", on a une zone de saisie pour indiquer le message du commit (message le plus précis possible afin de retrouver facilement les différentes versions du projet).

### git push : 
Afin de garder aussi ressemblant que possible le dépot local et le dépot distant, on va envoyer les modifications sur github avec la commande push.

### Exemples d'inaccessibilités :
- Parcours à effectuer avec navigation clavier
- Zoom à 200%
- Couper le son et regarder une vidéo sans sous-titres
- Contrastes insuffisants
- Couleurs porteuses d'information
- Animations innarêtables

___

## P1-J02

### Créer une sauvegarde VSCode :


- dans la sidebar de VSCode, on clique sur le logo git
- la liste des fichiers modifiés sont affichés
    - cliquer sur l'icone "plus" ➕
à côté d'un fichier pour ajouter les modifications de ce fichier
    - en haut, à côté de "Changes" (en anglais) pour ajouter les modifications de tous les fichiers
- renseigner un message décrivant les modifications
- ```Ctrl+Entrée``` ou ✔️ (juste au dessus) pour créer le commit (la sauvegarde)

- on peut vérifier la création du commit avec l'extension Git Graph
- on peut voir que notre commit apparait sur ```master``` (ou ```main```) mais pas sur ```origin/master```(ou ```origin/main```)
    - ```origin``` c'est le mot-clé pour le Remote Repository = dépôt distant = dépôt chez GitHub
    - donc il faut envoyer nos commits, nos sauvegardes sur GitHub (pour centraliser et avoir un backup)
    - dans la sidebar, cliquer sur les 3 petits points en haut à droite, puis cliquer sur "push"

- Pour vérifier que tout est ok, on rafraichit la page du navigateur 😉

### Utiliser ```checkout branch``` pour retrouver du code supprimé :


- afficher les commits avec Git Graph (click dans la barre d'état, en bas)
- retrouver le commit de la suppression de WordPress (s'il a bien été nommé, ce sera rapide)
- on veut avoir la sauvegarde juste avant celle-ci
- clic-droit sur la sauvegarde précédente, puis Checkout...
- confirmer
- le code source vient d'être modifié, le contenu est désormais celui à l'époque de la sauvegarde sélectionnée
- copier le texte nécessaire
- on peut alors retourner au dernier commit
    - retourner sur Git Graph
    - clic-droit sur le rectange ```master``` (ou ```main```)
    - cliquer sur ```Checkout branch...```
    - désormais, le code est revenu à la dernière sauvegarde effectuée
- on peut alors coller la partie Wordpress et ajouter les notes
- on crée une sauvegarde et on l'envoie sur GitHub

___

## P1-J03

## P1-J04

## P1-J05

## P2-J01

## P2-J02

## P2-J03

## P2-J04

## P2-J05