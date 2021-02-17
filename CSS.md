# CSS

## Sommaire

-
-
-

## IDs, Classes et CSS

Il existe deux types de sélecteurs CSS qu'il est important de comprendre, ```id``` et ```class```. Quand l'un ou l'autre de ces deux sélecteurs sont utilisés, cela nous permet d'appliquer un style à des éléments HTML d'une manière plus simple que simplement utiliser les règles CSS à l'intérieur de notre HTML.

- ```class``` : **L'attribut ```class``` n'est pas forcément unique pour des éléments HTML**. On peut avoir plusieurs fois la même ```class``` pour différents éléments HTML en utilisant ```class=""```. La syntaxe en CSS pour appeler une ```class``` est le point ```.```.

    *exemple* : 
```css
.exemple {

}
```


- ```id``` : **L'attribut ```id``` doit être unique à un élément HTML en particulier.** Il est définit à l'intérieur d'un élément HTML bien précis en utilisant ```id=""```. La syntaxe en CSS pour appeler un ```id``` est le hashtag ```#```.

    *exemple* :
```css
#exemple {

}
```
## 

___
## Les Boîtes ```inline``` et ```bloc```

En CSS, il existe deux type de boîtes : les boîtes en ```bloc``` et les boîtes ```inline```. Ces deux qualifications renvoient au comportement de la boîte au sein de la page et vis à vis des autres boîtes :

### Les boîtes en ```bloc```

Elles suivent les règles suivantes :

- La boîte s'étend en largeur pour remplir totalement l'espace offert par son conteneur. Dans la plupart des cas, la boîte devient alors aussi large que son conteneur, occupant 100% de l'espace disponible.
- La boîte occupe sa propre nouvelle ligne et créé un retour à la ligne, faisant ainsi passer les éléments suivants à la ligne d'après.
- Les propriétés de largeur (```width```) et de hauteur (```height```) sont toujours respectées.
- Les propriétés ```padding```, ```margin``` et ```border``` correspondantes respectivement aux écarts de remplissage interne, externe et à la bordure de la boîte auront pour effet de repousser les autres éléments.

À moins que l'on ne décide de changer le type de positionnement de la boîte en ```inline```, certains éléments tels que les titres (```<h1>```,```<h2>```, etc.) et les paragraphes (```<p>```) utilisent le mode ```bloc``` comme propriété de positionnement extérieur par défaut.

### Les boîtes en ```inline```

Elles suivent les règles suivantes :

- La boîte ne crée pas de retour à la ligne, les autres éléments se suivent donc en ligne.
- Les propriétés de largeur (```width```) et de hauteur (```height```) ne s'appliquent pas.
- Le padding, les marges et les bordures verticales (en haut et en bas) seront appliquées mais ne provoqueront pas de déplacement des éléments alentours.
- Le padding, les marges et les bordures horizontales (à gauche et à droite) seront appliquées et provoqueront le déplacement des éléments alentours.

Les éléments ```<a>```, utilisés pour les liens, ou encore ```<span>```, ```<em>``` et ```<strong>``` sont tous des éléments qui s'affichent en ```inline``` par défaut.

Le type de boîte appliqué à un élement est défini par la valeur de la propriété ```display``` tel que block ou inline, et se réfère à la valeur extérieur de positionnement.

___
## Propriétés des différents modèle de boîte

- Les propriétés qui définissent le flux du contenu dans une boîte :
```css
.exemple {
    overflow:
    overflow-x: 
    overflow-y:
}
```
- Les propriétés qui définiessent la taille d'une boîte :
```css
.exemple {
    height:
    width:
    max-height:
    min-height:
    max-width:
    min-width:
}
```
- Les propriétés qui définissent les marges d'une boîte :
```css
.exemple {
    margin:
    margin-bottom:
    margin-top:
    margin-left:
    margin-right:
    margin-trim:
}
```
- Les propriétés qui définissent le remplissage (```padding```) d'une boîte :
```css
.exemple {
    padding:
    padding-bottom:
    padding-top:
    padding-right:
    padding-left:
}
```
- Les autres propriétés :
```css
.exemple {
    box-shadow:
    visibility:
}
```

___
## Les modes de positionnement des boîtes

Une fois les boîtes générées, le moteur CSS doit les disposer les unes par rapport aux autres. Pour ce faire, il utilise un des algorithmes suivants :

- Le mode de positionnement ```normal``` positionne les boîtes les unes après les autres
- Le mode de positionnement ```flottant``` permet d'extraire une boîte du flux normal et de la placer sur le côté de la boîte englobante
- Le mode de positionnement ```absolu``` permet de placer une boîte dans un système de coordonnées absolues, basée sur l'élément englobant. Un élément positionné de façon absolue peut recouvrir d'autres éléments.

### Le mode ```normal```

Dans le mode de positionnement normal, les boîtes sont disposées les unes après les autres. Pour un contexte de mise en forme de bloc, elles seront empilées verticalement et pour un contexte de mise en forme en ligne, elles se suivront horizontalement. Le mode de disposition normal est déclenché lorsque la propriété CSS ```position``` vaut ```static``` ou ```relative``` et si la propriété CSS ```float``` vaut ```none```.

On a deux cas de figure pour le mode normal : le positionnement statique et le positionnement relatif.

- En positionnement statique (obtenu avec la valeur ```static``` pour la propriété ```position```), les boîtes sont dessinées à l'emplacement exact dicté par le flux normal.
- En positionnement relatif (obtenu lorsque la propriété ```position``` vaut ```relative```), les boîtes sont dessinées avec un décalage défini par les propriétés ```top```, ```bottom```, ```left``` et ```right```.

### Le mode ```flottant```

Avec le mode de positionnement flottant, certaines boîtes sont placées au début ou à la fin de ligne courante. Le texte (et tout ce qui se trouve dans le flux normal) épouse donc le contour des boîtes flottantes (sauf si la propriété ```clear``` dicte un autre comportement).

Pour qu'une boîte soit une boîte flottante, on utilisera la propriété ```float``` avec une valeur différente de ```none``` et la propriété ```position``` avec ```static``` ou ```relative```. Si ```float``` vaut ```left```, la boîte flottante sera positionnée au début de la ligne de la boîte englobante et si elle vaut ```right```, elle sera à la fin de la ligne.

### Le mode ```absolu``` 

En mode absolu, les boîtes sont entièrement retirées du flux normal et n'interagissent plus avec le flux. Elles sont positionnées de façon relative à leur bloc englobant grâce aux propriétés ```top```, ```bottom```, ```left``` et ```right```.

Un élément est positionné de façon absolue lorsque la propriété ```position``` vaut ```absolute``` ou ```fixed```.

Pour un élément positionné de façon fixe, le bloc englobant sera la zone d'affichage (viewport) et la position de l'élément est absolue par rapport à la zone d'affichage. Faire défiler le contenu ne modifie pas la position de l'élément.



