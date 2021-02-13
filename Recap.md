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

### Balisages et sémantiques - Markdown

#### Introduction

- langage de balisage : langage permettant de structurer ou mettre en forme des données en les organisant à l'aide de balises.
- Balises compréhensibles par un analyseur syntaxique (parser en anglais) --> interpréte le code et l'affiche.
- Fichiers HTML : lus par navigateurs Web.
- Particularité : la syntaxe est lisible d'elle-même : compris en le lisant, sans programme informatique.

#### Qu'est-ce qu'un fichier Markdown ?

- Format du fichier : .md
- Ouvrir dans VSCode
- Prévisualisation :
    - Cliquer sur l'icône en haut à droite "Ouvrir l'aperçu sur le côté"
    - raccourci ```Ctrl+Shift+V``` pour ouvrir l'onglet aperçu
    - raccourci ```Ctrl+K V``` (```Ctrl+K```, relâcher puis ```V```)

##### Aperçu : modifications en temps réel.

- Syntaxe de Markdown : caractères de ponctuation.

#### Pourquoi se servir de Markdown ?

- documentation de projets web (les fameux fichiers readme.md) : plus pratique pour écrire et modifier du texte, plus que le HTML.
- publier des contenus : blog, wikis, forums (comme Reddit…)

#### La syntaxe Markdown

- Ne se substitue pas au HTML,
- Fonctions réduites,
- Outil complémentaire. Possible d’insérer HTML dans Markdown.

#### Titres

2 syntaxes :

1. Dièse(s) + espace : jusqu'à 6 niveaux de sous-titres

```
# Titre 1
## Titre 2
### Titre 3
#### Titre 4
##### Titre 5
###### Titre 6
```

2. Signe égal et Tiret : 1 caractère suffit, mais 2 niveaux de titres possibles

```
Titre 1
===

Titre 2
------
```

#### Paragraphes

```
1 nouveau paragraphe : une ligne vierge.
```

#### Listes

- Liste non-ordonnée (à puces), trois syntaxes :

```
  + le signe plus

  - le tiret

  * un astérisque
```
```
- Liste 1
- Liste 2
- Liste 3
```

- Liste ordonnée (numérotées: chiffre suivi d’un point :

```
1. Liste 1
2. Liste 2
3. Liste 3
```

#### Remarque

Chiffre employé : aucune importance. Ex : 3 fois le chiffre 1 ou commencer par le chiffre 3 --> liste correctement numérotée.

#### Texte en gras et en italique

Syntaxe : **astérisques** :


- *Italique* (```*Italique*```)
- **Gras** (```**Gras**```)
- ***Gras et italique*** (```***Gras et italique***```)


#### Remarque

- Markdown : soulignement impossible :
    - Tendance délaissée sur le Web : hyperliens ==> texte souligné
    - Évite de souligner d’autres éléments pour éviter toute confusion.

#### Hyperliens

##### parenthèses et des crochets :

- texte du lien entre crochets ```[]```,

- URL entre parenthèses ```()```.

##### Exemple :

Code

```
Voici un exemple de lien : [Intitulé du lien](https://example.com/).
```

Résultat

Voici un exemple de lien : [Intitulé du lien](https://example.com/).

#### Citations

Signe supérieur à ```>```

Deux possibilités :

- Débuter chaque ligne par ```>```
- Insérer le signe ```>``` au début du paragraphe et terminer le paragraphe par une ligne vierge.

```
>Ceci est une **zone en retrait**.
>La zone en retrait continue ici.

>Ceci est une autre **zone de retrait**.
Cette zone continue sur cette ligne.

Cette ligne n’est pas en retrait.
```

Résultat :

>Ceci est une zone en retrait. La zone en retrait continue ici.

>Ceci est une autre zone de retrait. Cette zone continue sur cette ligne.

Cette ligne n’est pas en retrait.

#### Code

Syntaxe : **Backtick** ou apostrophe inversée (ne pas confondre avec les guillemets !) :

##### Code inline

Code à l'intérieur du paragraphe de texte, comme italique ou gras.

- **une apostrophe inversée au début et à la fin** du texte correspondant au code :

```
Cette phrase contient un terme en `code`.
```

Résultat :

##### Remarque

- Attention à ne pas écrire un accent grave (si caractère est suivi d'une voyelle) :
    - Une espace entre l’apostrophe inversée et la voyelle.

##### Code bloc

– Tout un bloc de texte :

- tabulation ```[Tab]```
- quatre espaces consécutives avant chaque ligne
- trois apostrophes inversée (début/fin bloc)

```
Ceci est un paragraphe classique.

  Ceci est la première ligne du bloc de code.
  	La seconde ligne est plus indentée que la première.
  Ceci est une autre ligne du bloc de code.

Ceci est un nouveau paragraphe classique.
```

```html
<html>
  <head> </head>
</html>
```

#### Ligne horizontale

- au minimum 3 fois de suite :
    - ```_``` (« tiret du bas »)
    - ```*``` (astérique)
    - ```-``` (« tiret haut »)

```
___

***

---
```

### Markdown et HTML

Markdown et HTML :

- Langages de balisage
- Structurer les éléments d'un document textuel (titres, paragraphes, listes, tableaux ou graphiques)

HTML :

- Lisible grâce à un navigateur Web (Firefox, Edge, Safari, Chrome, etc.)
- Possible d'écrire un fichier en Markdown > l'exporter au format HTML.

_Exercice pratique_ : Prévisualiser le code dans l'inspecteur :

- clic droit sur la page
- examiner l'élément
- Ou utiliser le raccourci clavier : Ctrl + Maj + C (ou Cmd + Maj + C sous Mac OS)

#### Sémantique HTML & accessibilité

##### Introduction rapide au HTML

Notions rapides sur les balises :

- Structurent le contenu de la page (texte, images, vidéos, tableaux, etc.)

- Nom des balises prédéfini dans les spécifications HTML : on ne peut pas en inventer !

- Utilisées pour leur valeur sémantique pas leur rendu visuel

- Deux balises marquent début et fin d'un élément : ```<nom-de-la-balise>``` et ```</nom-de-la-balise>```

- Pour certains éléments, la balise de fin n'est pas nécessaire, comme la balise image : ```<img />```

- Des éléments sans contenu existent, comme le saut de ligne : ```<br>```

    (On reviendra sur le HTML plus en détails en semaine 2, pas de panique !)

##### La Sémantique HTML

Le HTML est composé d'éléments sémantiques et d'éléments non sémantiques:

- Éléments sémantiques : communiquent la signification de leur contenu

- Éléments non sémantiques ne disent rien sur la signification de leur contenu.

##### Coder en HTML sémantique :

- Utiliser les éléments HTML pour communiquer une signification/des informations sur le contenu des documents Web plutôt qu'à des fins de présentation.
- Une grande partie des contenus web peut être rendue accessible grâce à l'utilisation d'éléments HTML appropriés !
- Ne demande pas plus de temps à écrire que du balisage non-sémantique

##### Coder en HTML non-sémantique :

- Une des principales causes des problèmes d'accessibilité sur le Web !

Repassons sur les éléments vus plus tôt en Markdown, dans leur version HTML.

#### Titres

Pour les titres, côté HTML, on remplace les signes dièse ```#``` par des balises ```<hN>```.

Décortiquons **la balise ouvrante** :

- La balise débute par le signe inférieur ```<```, comme toutes les balises HTML,
- La lettre ```H``` signifie « Headings » (Itres, en anglais, la vie est bien faire !),
- Suivie du chiffre situant le titre dans la hiérarchie des titres : de 1 à 6,
- Le signe supérieur ```>``` vient fermer la marche,
- Ce qui donne : ```<h1>``` dans le cas d'un titre de niveau 1.

##### La balise fermante :

- Presque identique à la balise ouvrante,
- On ajoute un signe ```/```(barre oblique) après le signe ```<``` pour signifier qu'il s'agit de la balise fermante,
- Résultat : ```</h1>``` pour fermer la balise de titre de niveau 1.

Les titres de niveau vont du niveau 1(```<h1>```) au niveau 6 (```<h6>```) :

- ```<h1>``` est utilisé pour représenter le titre au niveau le plus élevé,

- ```<h6>``` est utilisé pour représenter les titres au niveau le plus bas.

```html
<h1>Titre de niveau 1</h1>

<h2>Titre de niveau 2</h2>

<h3>Titre de niveau 3</h3>

<h3>Titre de niveau 3</h3>

<h4>Titre de niveau 4</h4>

<h2>Titre de niveau 2</h2>

<h3>Titre de niveau 3</h3>

<h4>Titre de niveau 4</h4>

<h5>Titre de niveau 4</h5>

<h6>Titre de niveau 4</h6>
```

##### Accessibilité

**Il est primordial de conserver une structure de titre cohérente !**

- Les personnes utilisant des lecteurs d'écran utilisent fréquemment les niveaux de titre pour déterminer rapidement le contenu de la page.
- Ne pas sauter un niveau de titre
- L'absence d'un titre intermédiaire pourrait amener le lecteur à se demander où le titre a été placé.

###### Exemple :

Passer d'un titre de niveau 2 à un titre de niveau 4 casserait la structure logique du document.

```
Cette structure de page n'est pas pertinente !

<h2>Titre de niveau 1</h2>

<h4>Titre de niveau 2</h4>

<h5>Titre de niveau 3</h5>
```

Les balises de titres doivent servir à :

- Indiquer les éléments titres d'un document
- Situer ces titres dans la structure logique de celui-ci

Les balises de titres **ne doivent pas servir** à :

- Afficher du texte de grande taille

- Utiliser une mise en forme jugée plus « jolie » que celle du titre approprié

**Le HTML ne doit pas être utilisé à des fins de mise en forme**, d'autres outils (styles CSS, guides de style) permettent de régler ces problèmes.

#### Paragraphes

Côté HTMl, les paragraphes sont signifiés par la balise ```<p>``` :

```
<h1>Titre de la page </h1>
<p>Ceci est un paragraphe.</p>

<p>Ceci est un nouveau paragraphe.</p>
```

##### Accessibilité

Répartir le contenu entre différents paragraphes permet d'améliorer l'accessibilité d'une page :

- Utilisateurs de lecteurs d'écran et autres outils d'assistance : permettent de naviguer de paragraphe en paragraphe (équivalent des espaces visuels pour des autres utilisateurs)
- Ne pas utiliser de paragraphes vides : les lecteurs d'écrans pourraient annoncer l'élément mais pas son contenu ce qui est source de confusion.

*Exemple* :

```
Cette structure de page n'est pas pertinente !

<p>Ceci est un paragraphe.</p>

<p> </p>

<p>Ceci est un nouveauparagraphe.</p>
```

Si besoin d'espacer les paragraphes : les propriétés CSS sont là pour ça ! (Vous le verrez en deuxième semaine)

#### Listes

##### Listes non ordonnées (à puces)

Une liste non ordonnées correspond à une liste d'éléments sans ordre particulier. Elle est souvent représentée par une liste à puces.

Pour insérer une liste non ordonnée :

- indiquer le type de liste à afficher, ici une liste non ordonnée : la balise correspondante est ```<ul>``` (unorderer list)
- Imbriquer chaque item de la liste dans la balise correspondante : ```<li>```
- Les balises ```li``` doivent être imbriquées dans la balise ```<ul>```

Ce qui donne :

```
<p>J'écris ma liste de courses :</p>

<ul>
<li>Clémentines</li>
<li>Pommes</li>
<li>Poires</li>
<li>Amandes</li>
</ul>
```

##### Listes ordonnées (à numéros)

Une liste ordonnées correspond à une liste numérotée.

Pour insérer une liste ordonnée :

- indiquer le type de liste à afficher, ici une liste ordonnée : la balise correspondante est ```<ol>```(unorderer list)
- Imbriquer chaque item de la liste dans la balise correspondante : ```<li>```
- Les balises ```li``` doivent être imbriquées dans la balise ```<ol>```

Ce qui donne :

```
<p>J'écris la liste de mes fruits de saison préférés :</p>
<ol>
<li>Clémentines</li>
<li>Poires</li>
<li>Amandes</li>
<li>Citron</li>
</ol>
```

Note : les numéros de la liste peuvent prendre la forme de nombres, de lettres, de chiffres romains ou de points. La mise en forme de la numérotation n'est pas utilisée dans la description HTML.

##### Accessibilité

Structurer correctement les listes dans des listes ordonnées ou non ordonées permet permet d'améliorer l'accessibilité d'une page :

- Utlisateurs de lecteurs d'écran et autres outils d'assistance : permettent de naviguer de liste en liste,
- Connaître le nombre d’éléments présents dans celle-ci,
- Naviguer plus facilement dans la liste : passer directement à la fin de la liste ou revenir au début de la liste,
- Ne pas créer de « fausses » listes à l'aide de tirets !

*Exemple* :

```
Cette liste n'est pas corectement structurée !

<p>J'écris la liste de mes fruits de saison préférés :</p>
<p>
– Clémentines
– Poires
– Amandes
– Citron
</p>
```

#### Texte en gras et en italique

##### Gras

L'élément HTML ```<strong>``` permet d'appliquer une emphase forte à un élément de texte. Cela se traduit généralement par un affichage en gras.

###### Pourquoi y a t'il plusieurs balises différentes ?

- La balise ```<strong>``` permet une mise en emphase forte :
    - C'est une balise avec une signification sémantique,
    - Visuellement, elle est souvent représentée par la mise en gras, mais elle peut tout aussi bien être passée en souligné, en surligné, en italique…
    - Ne pas utiliser la balise ```<strong>``` à des fins de présentation uniquement !

- La balise ```<b>```correspond à une mise en forme typographique :
    - Ce n'est pas une balise sémantique
    - Ne permet pas de séparer la forme du contenu
    - Ne pas l'utiliser : le style CSS est là pour la mise en forme

Ce qui donne :

```
<p>Je souhaite mettre une emphase forte sur <strong>les mots suivants</strong> dans mon paragraphe.</p>
```

##### Italique

Il y'a plusieurs manières de signifier l'italique en HTML. L'élément principal à retenir est ```<em>```:

- L'élément HTML ```<em>``` (pour emphase) est utilisé pour marquer un texte sur lequel on veut insister.
- ```<em>``` est habituellement affiché avec une police italique
- Il ne doit pas être utilisé pour appliquer un style italique uniquement !

Ce qui donne :

```
<p>Je souhaite mettre l'emphase sur <em>les mots suivants</em> dans mon paragraphe.</p>
```

Note :

- Il existe un élément permettant de marquer le titre d'une œuvre (livre, chanson, pièce, etc.) : la balise <cite>

#### Liens

Côté HTMl, les liens sont signifiés par la balise ```<a>``` (pour ancre, anchor en anglais). Cette balise sémantique permet d'indiquer un hyperlien vers :

- Un endroit différent de la page : on parle alors d'ancre,
- Une autre page Web.

Ce qui donne :

```
<h1>Titre de la page </h1>
<p>Ceci est un paragraphe contenant <a href="https://www.integra11y.fr/">un hyperlien vers le site d'Intégra11y</a>.</p>

<p>Ceci est un nouveau paragraphe.</p>
```

##### Accessibilité

**Ne pas confondre un lien et un bouton !**

- Un lien permet de se diriger vers un lieu :
    - vers une autre section d'une même page
    - Vers une page différente
- Un bouton permet une interaction de l'utilisateur avec le site, par exemple :
    - Intéragir avec un formulaire (Contact, questionnaire, …)
    - Déclencher l'affichage d'un élément masqué.

Les personnes qui utilisent TA, ont des troubles de la vision et/ou cognitifs peuvent être confuses lorsqu'un lien déclenche une action qui devrait être lancée par un bouton.

#### Citations

En HTML, une citation est indiquée par deux balises différentes, selon la longueur de la citation. Toutes deux sont des balises sémantiques :

- Citation longue : on utilise la balise ```<blockquote>```( bloc de citation, en anglais),
- Citation courte : on utilise la balise ```<q>```(pour *quote*, citation en anglais)

Ce qui donne :

```html
<blockquote>
	<p>Ceci est une citation longue..</p>
</blockquote>


<p>
  Ceci est <q>une citation courte</q>
</p>
```

#### Code

En HTML, on indique la présence d'un code dans un texte grâce à deux balises sémantiques :

- La balise ```<code>``` représente un fragment de code dans un texte
- La balise ```<pre>``` permet d'afficher plusieurs lignes de code.

Ce qui donne :

```html
<p><code>Ce texte est indiqué en tant que code.</code> Ce texte n'est pa sindiqué en tant que code.</p>

<pre>
	Ce texte est indiqué en tant que code.
	Ce texte est aussi indiqué en tant que code.
</pre>
```

#### Ligne horizontale

En HTML, la ligne horizontale a une signification sémantique :

- Elle signifie une pause significative dans la page;
- Elle est représentée par la balise ```<hr>``` (pour horizontal rule)

Ce qui donne :

```html
<p>
Les pandas roux sont géniaux. Ils sont mignons et tout doux.
</p>

<hr>

<p>
 Les poneys sont plus grands et moins exotiques, mais mignons aussi.
</p>
```

##### Accessibilité

Ne pas utiliser la balise ```<hr>``` à des fins de présentation, par exemple pour insérer une ligne horizontale pour « faire joli ». Le style CSS est là pour ça !

## P1-J04

### Git et les branches

Pour travailler proprement, on ne va pas utiliser la branche ```main``` pour le développement : git nous permet de créer d'autres branches dans le même projet !

C'est une bonne pratique, la branche ```main``` ne doit contenir qu'une version opérationnelle du projet, on va donc travailler, se tromper et corriger dans une branche à part pour ne pas abîmer le projet final.

#### 1. Récupérer le code

- on ouvre VSCode
    - on doit avoir accès au bouton ```Cloner un dépôt```.
    - si un dossier est ouvert au lancement, on le ferme (menu fichier / Fermer le dossier)
- on clone le projet en local.
- depuis le terminal la commande est : ```git clone adresse_du_dépot```

#### 2. Etude du projet

- avec Git Graph, on vérifie les branches et les commits existants
- on regarde ce qui a déjà été fait dans le fichier ```programme.md```.

#### 3. Création d'une nouvelle branche

On a plusieurs solutions pour créer une nouvelle branche

- avec Git Graph
    - on fait un click droit sur le commit de référence (le point de départ de la nouvelle branche)
    - on clique sur ```Create branch``` et on lui donne un nom
    - pour se positionner dessus, on peut cocher la case ```check out```
- avec le terminal
    - version longue :
        - on utilise la commande ```git branch <nom_branche>``` pour créer la branche
        - on se positionne dessus avec la commande ```git checkout <nom_branche>```
    - version courte :
        - on peut faire les 2 commandes en une seule : ```git checkout -b <nom_branche>```

Tous les commits qu'on fera par la suite se feront sur cette branche

#### 4. On avance le travail et on push sur Github

- on travaille comme d'habitude
    - on modifie le fichier ```programme.md```
    - on ajoute la version modifiée dans la zone de surveillance
    - on commit pour créer une nouvelle version du projet dans l'historique :
        - vérifier qu'on a bien enregistré tous les fichiers
        - on ajoute le ou les fichier(s) dans la zone de surveillance
            - sur VSCode
                - on clicque sur ```+``` dans le controle de code source
            - dans le terminal
                - on tape ```git add nom_fichier```
                - pour ajouter plusieurs fichiers/dossiers d'un seul coup, on peut taper ```git add .```
        - sur VSCode, dans controle du code source, on doit saisir un message aussi explicite que possible et taper Ctrl+entrée pour valider
        - dans le terminal, on peut taper la commande ```git commit -m "le message du commit"```
    - on push sur GitHub :
        - dans VSCode, controle du code source, sélectionner ```push``` dans le menu
        - dans le terminal, taper la commande ```git push```
          - pour pusher sur une autre branche que la branche principale (ou l'ajouter si elle n'existe pas encore), on doit indiquer son nom
          - ```git push origin nom_branche```

- on checke sur GitHub : les commits sont bien dans la nouvelle branche

#### 5. Pull Request

- une fois le travail terminé, on va proposer une mise à jour de la branche ```main```
- bonne pratique : faire vérifier son code par d'autres développeurs, on appelle ça une revue de code
    - on manque souvent de recul sur le code qu'on a produit
    - un regard neuf peut repérer plus facilement les fautes de syntaxe, d'orthographe ou les erreurs de logique
- GitHub nous propose un outil permettant aux développeurs d'échanger sur une modification proposée : ```la Pull Request```
- le propriétaire du projet va être averti qu'une modification est proposée
- il va pouvoir organiser la revue de code, laisser des commentaires pour le développeur afin qu'il corrige les erreurs
- quand tout le monde est d'accord, on peut fusionner la branche de développement avec la branche ```main``` : on fait un ```merge``` de la branche de dev dans ```main```
- dans ```main```, on a un nouveau commit qui contient toutes les modifications apportées

#### 6. Mise à jour du code en local après une PR (Pull Request)

- après la fusion (le merge), le code est à jour sur GitHub mais pas en local
- on va devoir récupérer le smodifications pour que le dépôt local et le dépôt distant contienne la même chose
- dans VSCode, on se positionne sur la branche main
    - avec Git Graph : click droit sur la branche et ```Checkout branch```
    - dans le terminal : ```git checkout main```
- on récupère les modifs avec un pull
- le graphe prend en compte les modifications

#### Mise à jour du code d'une branche de dev à partir de la branche principale

- si un autre développeur a créé une branche de son côté, il va devoir mettre à jour son code
- pour éviter les problèmes, il doit prendre en compte les modifications apportées à la branche ```main```
- git permet cette opération :
    - on se positionne sur la branche de dev :
        - avec Git Graph : click droit sur la branche et ```Checkout branch```
        - dans le terminal : ```git checkout <branche_dev>```
    - dans le terminal, on récupère les commits manquants avec un pull spécial : ```git pull origin main```
    - origin est le nom donné au dépôt distant, main désigne la branche qu'on veut rapatrier dans la branche de dev
- on peut vérifier le résultat sur le graphe, la branche de dev est au même niveau que la branche ```main```

#### Suppression d'une branche 

- une fois le travail effectué sur la branche de dev et la PR validée, on voudra souvent supprimer la branche de dev
- il faut être positionné sur une autre branche pour effectuer cette opération, on se place sur la branche ```main```
- pour cette opération, on doit de nouveau utiliser le terminal
- il faut supprimer la branche dans le dépôt local
    - ```git branch -d <nom_branche>```
- mais aussi dans le dépôt distant
    - ```git push origin --delete <nom_branche>```

## P1-J05

### Droits d'auteur

C'est la garantie légale que l'auteur restera propriétaire de son oeuvre En france (et dans plusieurs pays d'Europe), l'auteur et ses héritiers sont propriétaires d'une oeuvre jusqu'à 70 ans après le décès de l'auteur Au delà de ce délai, l'oeuvre passe dans le domaine public.

### Licenses

Plusieurs types de licences :

- commerciale
    - aucun droit de réutilisation ou de redistribution
    - sources du programme ne sont pas fournies
    - l'oeuvre est payante
- shareware
    - un peu moins restrctive
    - on pourra obtenir le produit gratuitement
    - limitations d'utilisation dans le temps ou au niveau des fonctionnalités
- libres
    - le logiciel est gratuit
    - on peut le modifier ou le réutiliser
    - on a tout de meme quelques restrictions selon la licence

[Les licences libres dans wikipédia](https://fr.wikipedia.org/wiki/Liste_de_licences_libres)

En tant que développeur web, on va surtout s'intéresser à la licence libre Creative Commons

De très nombreux contenus (images, vidéos, sons) vont etre placés sous cette licence par leurs auteurs Ils facilitent ainsi la reddiffusion de leur contenu en donnant des droits aux utilisateurs

[Creative Commons dans wikipédia](https://fr.wikipedia.org/wiki/Creative_Commons)

Pour trouver des contenus CC, on peut utiliser la fonction de filtre proposée par google

onglet images (ou videos), outils, droits d'usage et sélectionne Creative Commons

Toutefois, il nous manque des informations pour utiliser correctement (et légalement) les contenus

Le plus simple pour nous est d'utiliser le [moteur de recherche](https://search.creativecommons.org/) de la fondation CC

En sélectionnant un contenu sur ce site, on va avoir toutes les mentions obligatoires à indiquer sur notre site pour utiliser le contenu

Une autre solution est de rechercher des contenus libres de droit. Ces contenus pourront etre modifiés ou redistribués (gratuitement) par l'utilisateur

Plusieurs sites permettent de les retouver facilement :
- [flickr](https://www.flickr.com/explore)
- [pixabay](https://pixabay.com/fr/)
- [freeimages](https://www.freeimages.com/fr)
- [iconfinder](https://www.iconfinder.com/)
- [openclipart](https://openclipart.org/)

**Remarque** : certains contenus texte de sites web sont aussi placés sous licence CC

Cest le cas de Wikipédia, on va pouvoir réutiliser les textes des articles sous certaines conditions.

[Plus de détails ici](https://fr.wikipedia.org/wiki/Wikip%C3%A9dia:Citation_et_r%C3%A9utilisation_du_contenu_de_Wikip%C3%A9dia)

## P2-J01

### Découverte du langage HTML

Pour ouvrir l'inspecteur de code du navigateur : Raccourci ```F12``` ou via le clic droit "Inspecter l'élément".

#### Le HTML

C'est le fond. La forme c'est en CSS.

On fait attention à :

- La sémantique, c'est à dire l'utilisation des bons éléments HTML
- La hiérarchie de contenu formé par l'order logique des titres
- L'accessibilité

##### Syntaxe

- Syntaxe d'une balise d'ouverture : ```<html>```
- Syntaxe d'une balise de fermeture : ```</html>```
- Syntaxe d'une balise auto-fermante : ```<br />``` Dont l'espace + le slash final sont facultatif.

Un élément avec un attribut et une valeur :

```html
<html lang="fr">

</html>
```

#### Les éléments de base d'une page HTML


- Le ```Doctype``` pour déclarer le document
- ```html```, et son attribut ```lang```
- ```head``` pour les metadonnées
- La ```meta``` pour l'encodage de caractère avec l'attribut ```charset```
- Le ```title``` pour le titre de la page
- ```body``` pour le corps de page

```html
<!DOCTYPE html>
<html lang="fr">
  <head>
    <meta charset="UTF-8" />
    <title>Titre de ma page</title>
  </head>
  <body>
    
  </body>
</html>
```
(**Raccourcis Emmet** : ```!```)

#### Les éléments de structuration du contenu / éléments sectionnants

Ces balises sont obligatoire dans un document HTML 5 si ces zones existent :

- ```<header>``` : L'en-tête relatif à son parent (Le site ou un article)
- ```<nav>``` : Section de page représentant une liste de lien (Menu de navigation, fil d'Ariane)
- ```<main>``` : Le contenu principal du site, élément unique par page.
- ```<footer>``` : Le pied de page relatif à son parent (Le site ou un article)

Il existe ensuite d'autres, pas obligatoire mais très utiles :

- ```<section>``` : Section de page
- ```<article>``` : Élément indépendant (article de blog, projet dans un portfolio, post dans un forum, produit dans un e-commerce, commentaire, …)
- ```<aside>``` : Contenu relatif mais séparé du contenu principal (Sommaire de la page, texte secondaire)
- ```<address>``` : Information de contact relative à son élément parent, article ou body (Nom, adresse postale)
- Titre Hn : Titre de niveau 1 à 6

#### Quelques éléments sémantiques vus avec Markdown

Titres Hn, paragraphe ```<p>```, ```<strong>```, ```<em>```, listes ```<ul>``` / ```<ol>```, ```<br />```, ```<hr />```, ```<code>```, ```<blockquote>```.

#### Rôles ARIA

L'attribut ```role=""``` : "Landmarks Regions" que l'on pourrait traduire en "Régions clés".
Ce sont des rôles uniques à donner sur des zones précises du site.

- ```main``` : Sur le tag ```<main>```
- ```banner``` : Sur le tag ```<header>``` de l'en-tête du site (Pas sur les autre header dans la page)
- ```navigation``` : Sur le tag ```<nav>``` pour les navigations principales et secondaires du site uniquement
- ```contentinfo``` : Sur le tag ```<footer>``` du pied de page du site (Pas sur les autre footer dans la page)
- ```search``` : Sur la zone du moteur de recherche du site

#### Les commentaires

Entre les balises ```<html> </html>``` et pas en dehors.
Ne doit pas contenir de données sensible, car c'est visible dans le code source.

Syntaxe : ```<!-- Un commentaire en HTML -->```

```html
  <!--
    Un autre commentaire
    en
    HTML !
  -->
```
### Ressources

- [Liste des balises dites "auto-fermante"](https://html.spec.whatwg.org/multipage/syntax.html#void-elements)
- [Référence des éléments HTML](https://developer.mozilla.org/fr/docs/Web/HTML/Element)
- [Validateur HTML W3C](https://validator.w3.org/)

## P2-J02

### Introduction à CSS

CSS = Cascading Style Sheets

Permet de gérer la forme (l'apparence) de notre page HTML

- HTML : le fond (le gateau)
- CSS : la forme (la décoration autour du gateau + la cérise)

#### Ecrire du CSS

3 possibilités :

- directement dans la balise ciblée : ```<p style="color: red">Mon texte </p>```
- depuis la balise ```<style> </style>```
- depuis un fichier à part (monfichier.css) et ```<link rel="stylesheet" href="monfichier.css">``` (**raccourcis Emmet** : ```link:css```)

#### Contenu CSS vu en cours

```css
body {
  font-family: Courier;
}

h1 {
  text-align: center;
  border: 10px solid blue;
}

p {
  color: peru;
  font-size: 18px;
}

blockquote {
  background-color: gray;
  width: 300px;
  color: white;
}

blockquote p {
  color: white;
}

#citation-2 {
  background-color: tomato;
}

#experiences {
  font-family: 'Segoe UI';
}

.liste-2 {
  color: tomato;
}
```

#### Code couleurs

- [Retrouvez une liste de couleurs ici](https://developer.mozilla.org/fr/docs/Web/CSS/Type_color)

#### Nom de la couleur

```css
 p {
    color : red;
 }
```

#### Code Hexadécimal

Pour avoir une couleur au format Hexadécimal, on va utiliser le mot-clé '#' suivi de 6 caractères.

Chacun des 6 caractères ira de 0 à f : 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, a, b, c, d, e, f

- Noir : #000000
- Noir-gris : #555555
- Blanc : #ffffff

Couleurs primaires : Rouge - Vert - Bleu (RVB - RGB : Red Green Blue)

- Rouge : #ff0000
- Vert : #00ff00
- Bleu : #0000ff
- Jaune : #ffff00
- ff (Densité de couleur Rouge) 00 (Densité de couleur Vert) 00 (Densité de couleur Bleu)

```css
p {
    color:#ff0000;
}
```

#### Code RGB (Red Green Blue) - RVB (Rouge Vert Bleu)

```css
p {
    color:rgb(0,0,0);
}
```

rgb : on va lui donner des valeurs comprises entre 0 et 255

- Noir : rgb(0, 0, 0)
- Rouge : rgb(255, 0, 0)
- Vert : rgb(0, 255, 0)
- Blanc : rgb(255, 255, 255)

```css
p {
    color:rgb(255, 0, 0);
}
```

## P2-J03

## P2-J04

## P2-J05
