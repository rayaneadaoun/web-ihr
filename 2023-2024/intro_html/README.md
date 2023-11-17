# Introduction au langage HTML 

## Structure de base d'un fichier html 

```html
<!DOCTYPE html>

<html>

<head> 
    <meta charset="UTF-8">  <!-- Format des caractères du site -->
    <link rel="stylesheet" href="web.css">
    <title>Mon Site Web</title>  <!-- Titre qui apparait sur l'onglet du site -->
</head>

<body>
     <!-- je place mon code ici -->
</body>

</html>
```

## Balises html 

- Les balises sont les elements de bases du langage html, elles sont representées par un mot clé entourer de 2 chevrons, par exemple <p> , qui represente la balise paragraphe.  

- Une balise dit ouvrante est souvent accompagnée d'une balise jumelles dit fermantes , un peu comme des guillemets, voici un ex pour la balise p:  
```html  
<p> le contenu de la balise </p> 
```

### Balises de bases: 
```html 
<html> </html>  ->  il s’agit de la balise racine. 
<head> </head> ->  c’est la balise qui concerne l’en-tête de la page, elle contient des meta-données.
<body> </body> : elle concerne le corps de la page.

<header> </header> -> cette balise concerne le haut de page du document.
<footer> </footer> : cette balise concerne le pied de page du document.
<h1> </h1>, <h2> </h2>… : ce sont les balises titres. 
<p> </p> : cette balise permet de discerner un paragraphe d’un autre. 
<a> </a> : elles servent à entourer un lien, vers une autre donnée. 

<strong> </strong> : elle est utilisée pour mettre en gras un mot.
<br> </br> : ces balises servent à marquer un saut de ligne au sein d’un contenu textuel.
<u> </u> : celles-ci permettent de souligner un élément.
<i> </i> : permet de mettre en iatlique un mot ou groupe de mot.
<img src="" alt="" /> -> ajouter une image

# Balise de structures:
=> elles permettent de données une structure à notre document html , important pour mieux gerer le style avec css

<section> </section> -> L'élément HTML <section> représente une section générique d'un document, par exemple un groupe de contenu thématique

<div> <div> -> est un element de structuration qui n'a aucun effet sur le contenu, tant qu'il n'est pas utilisé par du css.

```
### Attributs
- Les éléments HTML ont des attributs ; ce sont des valeurs supplémentaires qui configurent les éléments ou ajustent leur comportement de différentes manières pour répondre aux critères souhaités par les utilisateurs.

- Les attibuts sont ajoutés à l'interieur des balises ouvrantes: 
```html
<img src="image1.jpg" alt="titre de l'image" />

src et alt sont les attribus de la balise <img> 

src -> permet d'ajouter le lien vers l'image
alt -> permet d'ajouter un titre à l'image 

Ici les attribus viennent enrichir la balise <img>
``` 
- Chaque balise accepte ou pas une certaines listes d'attribut, par exemple on ne pourrait pas ajouter l'attibut src à la balise p
```html 
<p src="test" > paragraphe 1 </p> => Ceci n'est pas possible
```

=> Il existe néomoins un attribut dit universel qui est accepter par toutes les balises, c'est l'attribut "class"  <=

- L'attribut class d'associer une balise à un type donné , le but et pouvoir mieux manipuler les balises en questions par CSS.
```html
<p class="fiction" > paragraphe de fiction </p>

<p class="classique" > paragraphe de litterature classique </p>

Grace à l'attribut "class" , je peux plus facilement distinguer les paragraphes de litterature classique de ce de fiction
```