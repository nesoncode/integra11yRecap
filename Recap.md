# Sommaire

- [Git](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#git-)

- [Créer une sauvegarde VSCode](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#créer-une-sauvegarde-vscode-)
  
- [Retrouver de code supprimé](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#utiliser-checkout-branch-pour-retrouver-du-code-supprim%C3%A9-)
  
- [Balisages et sémantiques - Markdown](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#balisages-et-sémantiques---markdown)
  
- [Markdown et HTML](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#markdown-et-html)
  
- [Git et les branches](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#git-et-les-branches)
  
- [Droits d'auteur](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#droits-dauteur)
  
- [Licenses](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#licenses)
  
- [Découverte du language HTML](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#découverte-du-langage-html)
  
- [Introduction à CSS](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#introduction-à-css)
  
- [Faire des liens](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#faire-des-liens)
- [Sélécteurs combinateurs](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#sélécteurs-combinateurs)
  
- [Spécificités CSS](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#spécificités-css)
  
- [Les images](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#les-images)
  
- [Modèle de boîte](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#modèle-de-boîte)

- [Positionner avec "position" et "float"](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#positionner-avec-position-et-float)

- [Positionner avec "display"](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#positionner-avec-display)


## Git :
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

[Sommaire](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#sommaire)
___

## Créer une sauvegarde VSCode :

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

[Sommaire](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#sommaire)
___
## Utiliser ```checkout branch``` pour retrouver du code supprimé :

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

[Sommaire](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#sommaire)
___
## Balisages et sémantiques - Markdown

### Introduction

- langage de balisage : langage permettant de structurer ou mettre en forme des données en les organisant à l'aide de balises.
- Balises compréhensibles par un analyseur syntaxique (parser en anglais) --> interpréte le code et l'affiche.
- Fichiers HTML : lus par navigateurs Web.
- Particularité : la syntaxe est lisible d'elle-même : compris en le lisant, sans programme informatique.

### Qu'est-ce qu'un fichier Markdown ?

- Format du fichier : .md
- Ouvrir dans VSCode
- Prévisualisation :
    - Cliquer sur l'icône en haut à droite "Ouvrir l'aperçu sur le côté"
    - raccourci ```Ctrl+Shift+V``` pour ouvrir l'onglet aperçu
    - raccourci ```Ctrl+K V``` (```Ctrl+K```, relâcher puis ```V```)

#### Aperçu : modifications en temps réel.

- Syntaxe de Markdown : caractères de ponctuation.

### Pourquoi se servir de Markdown ?

- documentation de projets web (les fameux fichiers readme.md) : plus pratique pour écrire et modifier du texte, plus que le HTML.
- publier des contenus : blog, wikis, forums (comme Reddit…)

### La syntaxe Markdown

- Ne se substitue pas au HTML,
- Fonctions réduites,
- Outil complémentaire. Possible d’insérer HTML dans Markdown.

### Titres

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

### Paragraphes

```
1 nouveau paragraphe : une ligne vierge.
```

### Listes

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

### Remarque

Chiffre employé : aucune importance. Ex : 3 fois le chiffre 1 ou commencer par le chiffre 3 --> liste correctement numérotée.

### Texte en gras et en italique

Syntaxe : **astérisques** :


- *Italique* (```*Italique*```)
- **Gras** (```**Gras**```)
- ***Gras et italique*** (```***Gras et italique***```)


### Remarque

- Markdown : soulignement impossible :
    - Tendance délaissée sur le Web : hyperliens ==> texte souligné
    - Évite de souligner d’autres éléments pour éviter toute confusion.

### Hyperliens

#### parenthèses et des crochets :

- texte du lien entre crochets ```[]```,

- URL entre parenthèses ```()```.

#### Exemple :

Code

```
Voici un exemple de lien : [Intitulé du lien](https://example.com/).
```

Résultat

Voici un exemple de lien : [Intitulé du lien](https://example.com/).

### Citations

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

### Code

Syntaxe : **Backtick** ou apostrophe inversée (ne pas confondre avec les guillemets !) :

#### Code inline

Code à l'intérieur du paragraphe de texte, comme italique ou gras.

- **une apostrophe inversée au début et à la fin** du texte correspondant au code :

```
Cette phrase contient un terme en `code`.
```

Résultat :

#### Remarque

- Attention à ne pas écrire un accent grave (si caractère est suivi d'une voyelle) :
    - Une espace entre l’apostrophe inversée et la voyelle.

#### Code bloc

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

### Ligne horizontale

- au minimum 3 fois de suite :
    - ```_``` (« tiret du bas »)
    - ```*``` (astérique)
    - ```-``` (« tiret haut »)

```
___

***

---
```

[Sommaire](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#sommaire)
___
## Markdown et HTML

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

### Sémantique HTML & accessibilité

#### Introduction rapide au HTML

Notions rapides sur les balises :

- Structurent le contenu de la page (texte, images, vidéos, tableaux, etc.)

- Nom des balises prédéfini dans les spécifications HTML : on ne peut pas en inventer !

- Utilisées pour leur valeur sémantique pas leur rendu visuel

- Deux balises marquent début et fin d'un élément : ```<nom-de-la-balise>``` et ```</nom-de-la-balise>```

- Pour certains éléments, la balise de fin n'est pas nécessaire, comme la balise image : ```<img />```

- Des éléments sans contenu existent, comme le saut de ligne : ```<br>```

    (On reviendra sur le HTML plus en détails en semaine 2, pas de panique !)

#### La Sémantique HTML

Le HTML est composé d'éléments sémantiques et d'éléments non sémantiques:

- Éléments sémantiques : communiquent la signification de leur contenu

- Éléments non sémantiques ne disent rien sur la signification de leur contenu.

#### Coder en HTML sémantique :

- Utiliser les éléments HTML pour communiquer une signification/des informations sur le contenu des documents Web plutôt qu'à des fins de présentation.
- Une grande partie des contenus web peut être rendue accessible grâce à l'utilisation d'éléments HTML appropriés !
- Ne demande pas plus de temps à écrire que du balisage non-sémantique

#### Coder en HTML non-sémantique :

- Une des principales causes des problèmes d'accessibilité sur le Web !

Repassons sur les éléments vus plus tôt en Markdown, dans leur version HTML.

### Titres

Pour les titres, côté HTML, on remplace les signes dièse ```#``` par des balises ```<hN>```.

Décortiquons **la balise ouvrante** :

- La balise débute par le signe inférieur ```<```, comme toutes les balises HTML,
- La lettre ```H``` signifie « Headings » (Itres, en anglais, la vie est bien faire !),
- Suivie du chiffre situant le titre dans la hiérarchie des titres : de 1 à 6,
- Le signe supérieur ```>``` vient fermer la marche,
- Ce qui donne : ```<h1>``` dans le cas d'un titre de niveau 1.

#### La balise fermante :

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

#### Accessibilité

**Il est primordial de conserver une structure de titre cohérente !**

- Les personnes utilisant des lecteurs d'écran utilisent fréquemment les niveaux de titre pour déterminer rapidement le contenu de la page.
- Ne pas sauter un niveau de titre
- L'absence d'un titre intermédiaire pourrait amener le lecteur à se demander où le titre a été placé.

##### Exemple :

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

### Paragraphes

Côté HTMl, les paragraphes sont signifiés par la balise ```<p>``` :

```
<h1>Titre de la page </h1>
<p>Ceci est un paragraphe.</p>

<p>Ceci est un nouveau paragraphe.</p>
```

#### Accessibilité

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

### Listes

#### Listes non ordonnées (à puces)

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

#### Listes ordonnées (à numéros)

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

#### Accessibilité

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

### Texte en gras et en italique

#### Gras

L'élément HTML ```<strong>``` permet d'appliquer une emphase forte à un élément de texte. Cela se traduit généralement par un affichage en gras.

##### Pourquoi y a t'il plusieurs balises différentes ?

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

#### Italique

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

### Liens

Côté HTMl, les liens sont signifiés par la balise ```<a>``` (pour ancre, anchor en anglais). Cette balise sémantique permet d'indiquer un hyperlien vers :

- Un endroit différent de la page : on parle alors d'ancre,
- Une autre page Web.

Ce qui donne :

```
<h1>Titre de la page </h1>
<p>Ceci est un paragraphe contenant <a href="https://www.integra11y.fr/">un hyperlien vers le site d'Intégra11y</a>.</p>

<p>Ceci est un nouveau paragraphe.</p>
```

#### Accessibilité

**Ne pas confondre un lien et un bouton !**

- Un lien permet de se diriger vers un lieu :
    - vers une autre section d'une même page
    - Vers une page différente
- Un bouton permet une interaction de l'utilisateur avec le site, par exemple :
    - Intéragir avec un formulaire (Contact, questionnaire, …)
    - Déclencher l'affichage d'un élément masqué.

Les personnes qui utilisent TA, ont des troubles de la vision et/ou cognitifs peuvent être confuses lorsqu'un lien déclenche une action qui devrait être lancée par un bouton.

### Citations

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

### Code

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

### Ligne horizontale

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

#### Accessibilité

Ne pas utiliser la balise ```<hr>``` à des fins de présentation, par exemple pour insérer une ligne horizontale pour « faire joli ». Le style CSS est là pour ça !

[Sommaire](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#sommaire)
___
## Git et les branches

Pour travailler proprement, on ne va pas utiliser la branche ```main``` pour le développement : git nous permet de créer d'autres branches dans le même projet !

C'est une bonne pratique, la branche ```main``` ne doit contenir qu'une version opérationnelle du projet, on va donc travailler, se tromper et corriger dans une branche à part pour ne pas abîmer le projet final.

### 1. Récupérer le code

- on ouvre VSCode
    - on doit avoir accès au bouton ```Cloner un dépôt```.
    - si un dossier est ouvert au lancement, on le ferme (menu fichier / Fermer le dossier)
- on clone le projet en local.
- depuis le terminal la commande est : ```git clone adresse_du_dépot```

### 2. Etude du projet

- avec Git Graph, on vérifie les branches et les commits existants
- on regarde ce qui a déjà été fait dans le fichier ```programme.md```.

### 3. Création d'une nouvelle branche

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

### 4. On avance le travail et on push sur Github

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

### 5. Pull Request

- une fois le travail terminé, on va proposer une mise à jour de la branche ```main```
- bonne pratique : faire vérifier son code par d'autres développeurs, on appelle ça une revue de code
    - on manque souvent de recul sur le code qu'on a produit
    - un regard neuf peut repérer plus facilement les fautes de syntaxe, d'orthographe ou les erreurs de logique
- GitHub nous propose un outil permettant aux développeurs d'échanger sur une modification proposée : ```la Pull Request```
- le propriétaire du projet va être averti qu'une modification est proposée
- il va pouvoir organiser la revue de code, laisser des commentaires pour le développeur afin qu'il corrige les erreurs
- quand tout le monde est d'accord, on peut fusionner la branche de développement avec la branche ```main``` : on fait un ```merge``` de la branche de dev dans ```main```
- dans ```main```, on a un nouveau commit qui contient toutes les modifications apportées

### 6. Mise à jour du code en local après une PR (Pull Request)

- après la fusion (le merge), le code est à jour sur GitHub mais pas en local
- on va devoir récupérer le smodifications pour que le dépôt local et le dépôt distant contienne la même chose
- dans VSCode, on se positionne sur la branche main
    - avec Git Graph : click droit sur la branche et ```Checkout branch```
    - dans le terminal : ```git checkout main```
- on récupère les modifs avec un pull
- le graphe prend en compte les modifications

### Mise à jour du code d'une branche de dev à partir de la branche principale

- si un autre développeur a créé une branche de son côté, il va devoir mettre à jour son code
- pour éviter les problèmes, il doit prendre en compte les modifications apportées à la branche ```main```
- git permet cette opération :
    - on se positionne sur la branche de dev :
        - avec Git Graph : click droit sur la branche et ```Checkout branch```
        - dans le terminal : ```git checkout <branche_dev>```
    - dans le terminal, on récupère les commits manquants avec un pull spécial : ```git pull origin main```
    - origin est le nom donné au dépôt distant, main désigne la branche qu'on veut rapatrier dans la branche de dev
- on peut vérifier le résultat sur le graphe, la branche de dev est au même niveau que la branche ```main```

### Suppression d'une branche 

- une fois le travail effectué sur la branche de dev et la PR validée, on voudra souvent supprimer la branche de dev
- il faut être positionné sur une autre branche pour effectuer cette opération, on se place sur la branche ```main```
- pour cette opération, on doit de nouveau utiliser le terminal
- il faut supprimer la branche dans le dépôt local
    - ```git branch -d <nom_branche>```
- mais aussi dans le dépôt distant
    - ```git push origin --delete <nom_branche>```

[Sommaire](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#sommaire)
___
## Droits d'auteur

C'est la garantie légale que l'auteur restera propriétaire de son oeuvre En france (et dans plusieurs pays d'Europe), l'auteur et ses héritiers sont propriétaires d'une oeuvre jusqu'à 70 ans après le décès de l'auteur Au delà de ce délai, l'oeuvre passe dans le domaine public.

## Licenses

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

[Sommaire](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#sommaire)
___
## Découverte du langage HTML

Pour ouvrir l'inspecteur de code du navigateur : Raccourci ```F12``` ou via le clic droit "Inspecter l'élément".

### Le HTML

C'est le fond. La forme c'est en CSS.

On fait attention à :

- La sémantique, c'est à dire l'utilisation des bons éléments HTML
- La hiérarchie de contenu formé par l'order logique des titres
- L'accessibilité

#### Syntaxe

- Syntaxe d'une balise d'ouverture : ```<html>```
- Syntaxe d'une balise de fermeture : ```</html>```
- Syntaxe d'une balise auto-fermante : ```<br />``` Dont l'espace + le slash final sont facultatif.

Un élément avec un attribut et une valeur :

```html
<html lang="fr">

</html>
```

### Les éléments de base d'une page HTML


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

### Les éléments de structuration du contenu / éléments sectionnants

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

### Quelques éléments sémantiques vus avec Markdown

Titres Hn, paragraphe ```<p>```, ```<strong>```, ```<em>```, listes ```<ul>``` / ```<ol>```, ```<br />```, ```<hr />```, ```<code>```, ```<blockquote>```.

### Rôles ARIA

L'attribut ```role=""``` : "Landmarks Regions" que l'on pourrait traduire en "Régions clés".
Ce sont des rôles uniques à donner sur des zones précises du site.

- ```main``` : Sur le tag ```<main>```
- ```banner``` : Sur le tag ```<header>``` de l'en-tête du site (Pas sur les autre header dans la page)
- ```navigation``` : Sur le tag ```<nav>``` pour les navigations principales et secondaires du site uniquement
- ```contentinfo``` : Sur le tag ```<footer>``` du pied de page du site (Pas sur les autre footer dans la page)
- ```search``` : Sur la zone du moteur de recherche du site

### Les commentaires

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

[Sommaire](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#sommaire)
___
## Introduction à CSS

CSS = Cascading Style Sheets

Permet de gérer la forme (l'apparence) de notre page HTML

- HTML : le fond (le gateau)
- CSS : la forme (la décoration autour du gateau + la cérise)

### Ecrire du CSS

3 possibilités :

- directement dans la balise ciblée : ```<p style="color: red">Mon texte </p>```
- depuis la balise ```<style> </style>```
- depuis un fichier à part (monfichier.css) et ```<link rel="stylesheet" href="monfichier.css">``` (**raccourcis Emmet** : ```link:css```)

### Contenu CSS vu en cours

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

### Code couleurs

- [Retrouvez une liste de couleurs ici](https://developer.mozilla.org/fr/docs/Web/CSS/Type_color)

### Nom de la couleur

```css
 p {
    color : red;
 }
```

### Code Hexadécimal

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

### Code RGB (Red Green Blue) - RVB (Rouge Vert Bleu)

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

### Ressources

- [Contrast Triangle](https://contrast-triangle.com/)
- [Tanaguru contrast finder](https://contrast-finder.tanaguru.com/)
- [Changer de couleur, MDN](https://developer.mozilla.org/fr/docs/Web/CSS/color)
- [Changer de taille de police, MDN](https://developer.mozilla.org/fr/docs/Web/CSS/font-size)
- [Définir les polices de caractères, MDN](https://developer.mozilla.org/fr/docs/Web/CSS/font-family)
- [Définir la graisse utilisée pour le texte, MDN](https://developer.mozilla.org/fr/docs/Web/CSS/font-weight)
- [Aligner du texte, MDN](https://developer.mozilla.org/fr/docs/Web/CSS/text-align)
- [Modifier le rendu d'un texte, MDN](https://developer.mozilla.org/fr/docs/Web/CSS/text-transform)
- [Définir la bordure d'un élément HTML, MDN](https://developer.mozilla.org/fr/docs/Web/CSS/border)

[Sommaire](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#sommaire)
___
## Faire des liens

### Syntaxe

Syntaxe simple d'un lien :
```<a href="https://duckduckgo.com">DuckDuckGo</a>```

L'ancre :

```html
<a href="#ancre">Lien vers mon ancre</a>

<section id="ancre">
  <p>Du contenu ici</p>
</section>
```

Un lien dans un nouvel onglet :
```<a href="https://duckduckgo.com" title="DuckDuckGo - Nouvelle fenêtre" target="_blank">DuckDuckGo</a>```

### Relatif et absolu

**Absolu** :
URL complète ```https://www.integra11y.fr/programme.php```

**Relatif** :
Chemin vers la page voulue, relatif à la position actuelle.
Depuis la page d'accueil à la racine : ```./programme.php.```

### Lien interne et lien externe

**Lien interne** :
Lien vers le site courant.
Lien relatif de préférence sauf exception : Si le contenu doit paraitre dans un flux RSS.

**Lien externe** :
Lien vers une adresse différente.
Lien absolu uniquement.

#### Mail et téléphone

Pour rendre une adresse mail ou un numéro de téléphone cliquable.

**Mail** : ```<a href="mailto:contact@exemple.fr">contact@exemple.fr</a>```

**Tel** : ```<a href="tel:+33607080910">06 07 08 09 10</a>```

### Pseudo classes CSS pour les différents états des liens


- ```:visited``` : Lien déjà visité (se base sur l'historique de navigation)
- ```:active``` : Élément actif (clic appuyé), si besoin d'indiquer qu'un élément est appuyé. Sur un lien menant vers une page ou un document, l'effet sera probablement peu visible.
- ```:hover``` : Survolé (à l'aide de la souris)
- ```:focus``` : Focus (Prise de contrôle de l'élément, au clic ou via une tabulation)
- ```:link``` : Les liens n'ayant pas encore été visités (Ça ne veut pas dire style par défaut)

### Le style du focus

Naviguation au clavier avec les touches ```tab```, et ```Maj``` ```tab``` pour revenir en arrière.

Le style de focus par défaut peut-être supprimé à condition d'être remplacé par une autre solution adéquate **visible**.<br/>
**On ne supprime pas totalement le style de focus** sous peine de rendre impossible la navigation au clavier en cachant la position courante. On recommande de laisser le style par défaut, ou bien de mettre un autre style avec la propriétée ```outline``` en CSS, en respectant le ratio de contraste 3:1 avec la couleur de fond de la page.

### Identifier un lien 

Un lien doit être identifiable parmi le contenu qui l'entoure.<br/>
Si on choisit d'avoir uniquement une couleur différente pour les liens, le ratio de contraste entre le lien et le texte qui l'entoure doit être d'au moins 3:1. Mais en plus, le ratio de contraste pour le lien doit être d'au moins 4,5:1 avec la couleur de fond. On peut s'aider de [cet outil](https://contrast-triangle.com) pour calculer le constraste de couleur.

[Sommaire](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#sommaire)
___
## Sélécteurs combinateurs

Différents sélecteurs combinateurs :

- Sélecteur de descendants : ```div span```
- Sélecteur de descendants direct : ```ul > li```
- Sélecteur de voisins : ```p ~ span```
- Sélecteur de voisin direct : ```div + p```

Il n'y a pas de sélecteur ascendant (Sélectionner un parent à partir d'un enfant).

[Sommaire](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#sommaire)
___
## Spécificités CSS

La spécificité détermine quelles règles CSS sont appliquées par les navigateurs. Par exemple, lorsque deux sélecteurs s'appliquent au même élément, c'est celui qui a la plus grande spécificité qui l'emporte.

### Hiérarchie des spécificités

1. Les styles inline
2. Les ```id```
3. Les classes, atributs et pseudos-classes
4. Éléments et pseudos-éléments

Attention à l'usage de ```!important``` !

### Ressources

- [Spécificité, MDN](https://developer.mozilla.org/fr/docs/Apprendre/CSS/Building_blocks/Cascade_et_heritage#sp%C3%A9cificit%C3%A9_2)

Sites pratiques pour calculer la spécifité des sélecteurs :

- [Code Captain](https://www.codecaptain.io/tools/css-specificity-calculator)
- [Polypane](https://polypane.app/css-specificity-calculator/)
- [Keegan](https://specificity.keegan.st/)

[Sommaire](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#sommaire)
___
## Les images

### src

```<img src="./mon-image.jpg">```

### width et height

Les attributs ```width``` et ```height``` correspondent bien à l'espace alloué à l'image sur la page, et l'image appelée n'est pas sur-dimensionnée pour éviter des problèmes de performance, ni sous-dimensionnée pour qu'elle reste nette.

### alt

Distinguer une image informative et une image décorative :<br/>
**Informative** : Je remplis l'attribut alt.<br/>
**Décorative** : Je mets l'attribut alt mais je le laisse vide : ```alt=""```.<br/>

L'attribut ```alt``` est donc **toujours présent** sur une image.<br/>
Si l'alternative est trop longue ou trop complexe, la description est ajoutée dans la page, un lien peut-être fait avec l'atribut ```longdesc``` vers cette description.

### Lien images

Si le lien ne contient qu'une image, c'est le alt qui peut servir d'intitulé.

```html
<a href="index.html">
  <img src="./home.png" alt="Accueil" width="64" height="64">
</a>
```

Ou bien avec ```title``` si l'intitulé du lien n'est pas suffisant (on reprends l'intitulé du lien + une information supplémentaire utile) :

```html
<a href="index.html" title="Integra11y (retour à l’accueil)">
  <img src="./integra11y.png" alt="Integra11y" width="64" height="64">
</a>
```

### Lien composite

On évite de faire deux lien adjacents identiques (lien image et lien texte). Faisons plutôt un lien composite pour éviter la redondance.
Ici c'est ce qu'on appelle un "lien composite", un lien contenant à la fois du texte et un ou plusieurs enfants de type image.
Si le lien contient un intitulé explicite, l'image est alors plutôt décorative et on garde le ```alt``` vide.

```html
<a href="index.html">
  <img src="./home.png" alt="">
  Accueil
</a>
```

### Vérifier ses attributs alt

Avec l'extension navigateur Web Developer, dans l'onglet "images" puis : "Display Alt Attributes".

[Sommaire](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#sommaire)
___
## Modèle de boîte

### Modèles de boîte :

- **Par défaut** : ```box-sizing: content-box;``` - La taille de la boite de contenu
- **Alternatif** : ```box-sizing: border-box;``` - La taille de la boite de contenu + ```padding``` + ```border``` compris.

Attention, ```padding-box``` est obsolète.

Astuce pour utiliser ce modèle de boîte alternatif partout sur le site :

```css
html {
  box-sizing: border-box;
}

*, *::before, *::after {
  box-sizing: inherit;
}
```

### margin, padding, border

Sur les éléments de type inline :

- ```width``` et ```height``` sont ignorées
- ```padding```, ```margin``` et ```border``` appliquées verticalement ne provoque pas de déplacement des éléments alentours
- ```padding```, ```margin``` et ```border``` appliquées horizontalement provoque le déplacement des éléments alentours

Sur les éléments de type bloc :

- ```width``` et ```height``` sont appliqués
- ```padding```, ```margin``` et ```border``` sont appliqués en provoquant le déplacement des éléments alentours

La valeur ```auto``` sur sa propriété margin permet de donner des marges qui prennent la place disponible. Dès lorsque l'on spécifie une taille (```width```) à l'élément de type bloc, les marges de droite et de gauche en ```auto``` vont permettre de centrer l'élément.

### Fusion de marge

Les marges verticales fusionnent sur les éléments de type bloc, en prenant la valeur la plus grande :

- Entre éléments adjacents
- Entre éléments parents / enfants

[Sommaire](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#sommaire)
___
## Positionner avec "position" et "float"

### Définition du flux

Flux = ordre dans lequel les éléments HTML sont placés les uns après les autres dans le code de la page. Les éléments s'affichent dans l'ordre où ils sont déclarés dans le code HTML. C'est donc **la position par défaut**.

### Différents types de positionnement avec ```position```

#### Le positionnement "static"

- Positionnement par défaut de chaque élément — cela veut tout simplement dire « positionner l'élément selon le cours normal de placement — rien de spécial à voir ici ».
- N'a aucun effet sur un élément si on ajoute cette propriété.

#### Le positionnement "relative"

- Permet de décaler un élément par rapport à sa position par défaut dans la page.
- Doit être combinée avec les propriétés ```top```, ```bottom```, ```left``` et ```right```.
- Utilisé seul, il permet de créer créer un parent positionné pour les éléments enfants et descendants positionnés en absolu.

#### Le positionnement "absolute"

- Un élément positionné en absolute **est retiré du flux normal de la page**.
- On utilise aussi les propriétés top, bottom, left et right pour le positionner.
- Par défaut, l'élément absolu se positionne par rapport à l'élément ```<htlml>```.
- On peut **changer ce contexte de positionnement** en ajoutant ```position: relative``` à un élément ancêtre (parent ou plus lointain).

#### La propriété ```z-index```

- Permet de modifier l'ordre des éléments qui se superposent, indépendemment de leur place dans le code source.
- Ne marche qu'avec des éléments positionnés (en relative, absolute, fixed ou sticky).

#### Le positionnement "fixed"

- Comme pour le positionnement absolu, l'élément fixed est lui aussi retiré du flux normal de la page.
- Mais l'élément est toujours positionné par rapport à la fenêtre du navigateur.
- Les éléments en position fixe ne bougent plus lorsque le document est scrollé.

#### Le positionnement "sticky"

- C'est un **croisement entre position relative et position fixe**.
- Le positionnement sticky s’effectue par rapport à la position de son conteneur, et non pas la fenêtre du navigateur.
- Le positionnement sticky démarre à partir d'un seuil défini (ex: à partir de 10px du haut de la fenêtre) :
  - l'élément se positionnera dans le flux normal de la page jusqu'à ce que le viewport défile au point où l'élément est à moins de 10 pixels du haut.
  - Ensuite, il sera fixé à 10 pixels du haut, jusqu'à ce que le viewport redéfile jusqu'avant ce seuil.

#### Les flottants

- La propriété ```float``` permet d'implémenter une image flottant dans une colonne de texte.
- L'élément possèdant la propriété ```float``` est **retiré du flux normal de la page** et collé du côté de son conteneur parent.
- Tout contenu disposé après l'élément flottant dans le cours normal de page (c'est à dire disposé à la suite dans le code source) va maintenant l'envelopper en remplissant l'espace sur toute sa hauteur.
- On peut dégager un élément, c'est-à-dire l'empêcher de remonter pour se placer à côté du flottant avec la propriété ```clear```

#### Le "clearfix hack"

- Pour certains designs, on souhaite que l'élément flottant ne dépasse pas de son conteneur et avoir une couleur de fond ou une bordure autour du texte et de l'image. Pour ça, on utilise le clearfix hack, avec le pseudo-élément ```::after```.

### Accessibilité et positionnement

Attention aux points suivants lorsqu'on utilise le positionnement en CSS :

- l'ordre des contenus qui doit être cohérent dans le code source.
- les risques de superposition du contenu au zoom texte, graphique ou lors de l'agrandissement des caractères

[Sommaire](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#sommaire)
___
## Positionner avec "display"

### Rappel sur les éléments "inline" et "block"

Les éléments HTML ont tous un mode d'affichage par défaut : "inline" et "block". Pour rappel :

- [la liste des éléments de type "inline"](https://developer.mozilla.org/fr/docs/Web/HTML/%C3%89l%C3%A9ments_en_ligne#liste_des_%C3%A9l%C3%A9ments_en_ligne) (documentation MDN)
- [la liste des éléments de type "block"](https://developer.mozilla.org/fr/docs/Web/HTML/%C3%89l%C3%A9ments_en_bloc#%C3%A9l%C3%A9ment_de_bloc_ou_%C3%A9l%C3%A9ment_en_ligne) (documentation MDN)

Certaines propriétés CSS n'ont pas d'effet sur les éléments inline : ```width```, ```height```, ```margin-top``` et ```margin-bottom```.

### Modifier le rendu d'un élément

On peut modifier le mode d'affichage par défaut d'un élément grâce à la propriété ```display``` :

- ```display: block;``` : pour transformer le mode d'affichage d'un élément en "block"
- ```display: inline;``` : pour transformer le mode d'affichage d'un élément en "inline"
- ```display: inline-block;``` : pour placer des éléments les uns à côté des autres (comme inline) tout en permettant d'utiliser les propriétés CSS de hauteur, largeur et marges

On peut centrer horizontalement des éléments en ```inline-block``` en utilisant la propriété ```text-align: center;``` sur le parent.

On peut gérer l'alignement vertical des éléments de type "inline" ou modifiés par la propriété ```display: inline-block;``` grâce à la propriété ```vertical-align.```

### Conclusion générale sur le positionnement

#### Les erreurs à ne pas commettre

- Ne pas utiliser la propriété ```position``` à tort et à travers, la majorité des positionnements en CSS peuvent s'effectuer sans cette propriété.
- Ne pas tout positionner en "absolute" : c'est un positionnement à la fois puissant et limité qui doit être utilisé ponctuellement.

#### Quels types de positionnement utiliser en priorité ?

- Garder les éléments dans le flux, jouer sur les marges internes et externes
- Modifier le mode de rendu avec la propriété ```display```.
- ```float``` pour faire flotter du texte autour d'un élément (pas pour des mises en page complètes)
- Utiliser le positionnement absolu dans les conditions suivantes :
  - si on sait positionner un élément en absolu par rapport à son parent ou ancêtre positionné
  - si on a une idée précise des conséquences du positionnement absolu (risque de chevauchement des contenus)
  - si on sait à l'avance quels sont les contenus qui seront ainsi positionnés, et si ces contenus ne risquent pas d'être augmentés et ainsi de déborder de l'espace défini.
- Utiliser le positionnement relatif principalement pour :
  - créer un parent positionné pour les éléments enfants et descendants positionnés en absolu
  - décaler de quelques pixels un élément par rapport à sa position normale. Si vous écrivez ```position: relative; top: -356px;```, c'est probablement qu'il est mal utilisé.
- Utiliser le positionnement fixe en connaissance de cause, en prenant bien attention de le tester sur différentes tailles d'écran et au zoom.

[Sommaire](https://github.com/nesoncode/integra11yRecap/blob/main/Recap.md#sommaire)
___
