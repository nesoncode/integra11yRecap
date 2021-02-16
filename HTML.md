# HTML

## Sommaire

-
-
-

## La tête de site (```<head></head>```)

Fournit des **informations générales (métadonnées)** sur le document, incluant son titre et des liens ou des définitions vers des scripts et feuilles de style. 

## Le corps de site (```<body></body>```)

Représente le contenu principal du document HTML. **Il ne peut y avoir qu'un élément ```<body>``` par document.**<br/>
Au sein de cet élément ```<body>``` on trouve différentes sections :

### L'en-tête du site (```"<header></header>"```)

Il s'agit généralement d'un grande bande horizontale, située **en haut** du site avec un grand titre et/ou un logo. C'est à cet endroit qu'on a **toujours la même information sur le site**, quelle que soit la page du site sur laquelle on est.

### La barre de navigation (```<nav></nav>```)

Celle-ci permet de **faire référence aux différentes sections du site** via des menus ou des onglets. Comme pour l'en-tête, la barre de navigation sera généralmeent présente sur l'ensemble du site. De nombreux concepteurs web considèrent que la barre de navigation **fait partie intégrale de l'en-tête** mais ce n'est pas strictement nécessaire.

### Le contenu principal (```<main></main>```)

Une zone importante, **située au centre** dont le contenu est spécifique selon la page visitée.<br/> 
Il peut être segmenté de manière logique grâce à :

#### Les articles (```<article></article>```)

Représente du **contenu autonome dans un document, une page, une application, ou un site**. Ce contenu est prévu pour être distribué ou réutilisé indépendamment.

#### Les sections (```<section></section>```)

Représente une **section générique d'un document**, par exemple un groupe de contenu thématique. Une section **commence généralement avec un titre**.

### Le panneau (```<sidebar></sidebar>```)

Il contient des informations périphériques, des liens, des citations, des publicités. Généralement, ce panneau dépend du contenu principal de la page mais **on trouve également des panneaux latéraux qui agissent comme des menus de navigation** secondaires.

### Le pied de page (```<footer></footer>```)

C'est ici qu'**on trouvera les informations de contact, de copyright…** C'est un endroit où on place **des informations communes à l'ensemble du site mais qui ne sont pas primordiales** pour le site en tant que tel. Le pied de page est parfois utilisé par les outils de référencement afin de fournir un accès rapide à certaines parties du site.

## Les rôles ARIA

[ARIA](https://developer.mozilla.org/fr/docs/Glossaire/ARIA) est une méthode qui **permet d'indiquer aux technologies d'aide à la navigation qu'un élément HTML possède des fonctionnalités web applicatives.**

- ```<main role="main">```
- ```<header role="banner"```
- ```<nav role="navigation">```
- ```<aside role="complementary">```
- ```<footer role="contentinfo">```

## Les éléments de type "bloc"

**Occupe toute la largeur disponible**. Lorsque 2 éléments blocs se suivent dans une page, ils sont positionnés (par défaut) l'un sous l'autre. Les balises de type ```bloc``` sont des **boites d'éléments qui peuvent contenir des éléments orphelins** (comme du texte, simples caractères...), **des balises de type ```inline```**, **des balises de type ```autofermante```** et même d'autres balises de type ```bloc```. 

- La tête de site : ```<head></head>```
- Le corps de site : ```<body></body>```
- Titres : ```<h1></h1>``` (jusqu'a 6 au total)
- Paragraphes : ```<p></p>```
- Listes ordonnées  : ```<ol></ol>```
- Listes non-ordonnées : ```<ul></ul>```
- Eléments de listes : ```<li></li>```
- Listes avec définition : ```<dl></dl>```
- Définitions : ```<dt></dt>```
- Titres de définition : ```<dd></dd>```
- Diviseurs : ```<div></div>```
- Blocs de citation : ```<blockquote></blockquote>```
- Tableaux : ```<table></table>```
- Blocs de code préformatés : ```<pre></pre>```
- Formulaires de saisie : ```<form></form>```
- Eléments de figure : ```<figure></figure>```

## Les éléments de type "inline"

Les balises de type ```inline``` ne **peuvent contenir que des éléments orphelins** (texte...), d'**autres balises ```inline```**, mais pas de balises de type ```bloc```.

- Ancres : ```<a></a>```
- Balises multi-usage : ```<span></span>```
- Gras (texte) : ```<strong></strong>```
- Italique (texte) : ```<em></em>```
- Element de citation : ```<cite></cite>```
- Element de légende d'un tableau : ```<caption></caption>```
- Element de légende d'une figure : ```<figcaption></figcaption>```
- Signaler une abbréviation : ```<abbr></abbr>```
- Eléments de code en incise : ```<code></code>```
- Eléments de titre : ```<titre></titre>```

## Les éléments de type "autofermants"

Les balises de type ```autofermants``` sont des **balises qui sont ouvrantes et fermantes en même temps**. Cela signifie qu'elles **ne contiennent pas de contenu**. On ferme donc la balise en ajoutant un espace et un slash (```/```) à la fin de la balise.

- Sauts de ligne : ```<br />``` (également ```inline```)
- Champs de saisie dans un formulaire : ```<input />```  (également ```inline```)
- Images : ```<img />``` (également ```inline```)
- Eléments de lien : ```<link />``` (également ```inline```)
- Eléments de rupture thématique : ```<hr />``` (également ```bloc```)

### Ressources

- [Découper une page web en sections logiques, MDN](https://developer.mozilla.org/fr/docs/Apprendre/HTML/Comment/D%C3%A9couper_une_page_web_en_sections_logiques)
- [Les niveaux ou "types" d'éléments HTML block et inline](https://www.pierre-giraud.com/html-css-apprendre-coder-cours/block-inline/)