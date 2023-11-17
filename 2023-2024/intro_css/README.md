# Introduction au langage CSS

Le CSS correspond à un langage informatique permettant de mettre en forme des pages web HTML .

- La balise <link>  dans un fichier html permet de faire le lien avec un fichier css
```html
<head>
    
    <link rel="stylesheet" href="web.css">
    
</head>
```


## Structure d'un fichier css
- Si par exemple je veux appliquer une certaines mise en forme sur les balises "h1" de mon fichier html, par exemple changer leurs couleurs.  

Fichier html
```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <link rel="stylesheet" href="web.css">
    <title>Mon Site Web</title>
</head>
<body>
    <header>
        <h1>Mon Site Web</h1>
    </header>
</body>
</html>
``` 
Fichier CSS (web.css)
```css
h2 {
    color: red ;
}
```
- Css permet d'appliquer un style sur des balises html definies grace à ce que l'on appelle des "regle", dans notre exemple la regle "color" , permet de changer la couleur de l'element souhaité
```css
h2 <---- type de balise sur laquelle la regle va s'appliquer
{
    color:   red ;
    ↑          ↑
regle css     valeur de la regle
}

les " ; " est important apres chaque regle
On peut appliquer pour un meme type de balise plusieurs regles au meme temps

```

## Regles CSS


* Arrière-plan

    [background-color](https://developer.mozilla.org/fr/docs/Web/CSS/background-color) -> couleur de fond d'un element

    [background-image](https://developer.mozilla.org/fr/docs/Web/CSS/background-image) -> définir une ou plusieurs images comme arrière(s)-plan(s)

* Bordure

    [border-color](https://developer.mozilla.org/fr/docs/Web/CSS/border-color)

    [border-style](https://developer.mozilla.org/fr/docs/Web/CSS/border-style)

    [border-width](https://developer.mozilla.org/fr/docs/Web/CSS/border-width)

* Espacement/visibilité/positionnement/taille

    [display](https://developer.mozilla.org/fr/docs/Web/CSS/display)

    [float](https://developer.mozilla.org/fr/docs/Web/CSS/float)

    [margin](https://developer.mozilla.org/fr/docs/Web/CSS/margin)

    [padding](https://developer.mozilla.org/fr/docs/Web/CSS/padding)

    [width](https://developer.mozilla.org/fr/docs/Web/CSS/width)

    [height](https://developer.mozilla.org/fr/docs/Web/CSS/height)


* Police

    [font-family](https://developer.mozilla.org/fr/docs/Web/CSS/font-family)

    [font-size](https://developer.mozilla.org/fr/docs/Web/CSS/font-size)

    [font-style](https://developer.mozilla.org/fr/docs/Web/CSS/font-style)

    [font-weight](https://developer.mozilla.org/fr/docs/Web/CSS/font-weight)

* Texte

    [color](https://developer.mozilla.org/fr/docs/Web/CSS/color)

    [text-align](https://developer.mozilla.org/fr/docs/Web/CSS/text-align)

    [text-decoration](https://developer.mozilla.org/fr/docs/Web/CSS/text-decoration)

    [text-indent](https://developer.mozilla.org/fr/docs/Web/CSS/text-indent)

## Selecteurs et attributs 
- Rappelez vous , nous avons vu l'attribut html "class" qui permet d'identifier un element html en lui donnant un type
```html
Rappel attribut class

<p class="fiction" > paragraphe de fiction </p>

```

- Grace à l'attribut class on peut en css appliqués une regle sur des elements html qui sont categorisés par une classe en particulier sans avoir a modifier les autres elements html de la meme balise.

Dans cette exemple j'ai 2 balises "p" dans mon code html.
```html
<p class="fiction" > paragraphe de fiction </p>

<p class="classique" > paragraphe de litterature classique </p>

```
Et je voudrais modifier la couleur de la premiere balise "p" uniquement, si j'utilise le selecteur p dans mon code css cela appliquera la modification au 2 balises "p" de mon code html.
```css
p {
    color: red ;
}
```
Ce code css ne nous permet pas de faire ce que l'on veut. 

- Par contre grace à l'attribut "class" present sur la premiere balise "p" , je peux en css cibler uniquement les elements d'une "class" donnée, grace au code css suivant.

```css
.fiction {
    color: red ;
}
```
- Grace a ce dernier code css uniquement les balises contenant l'attribut "class" avec la valeur "fiction" seront modifiées. 