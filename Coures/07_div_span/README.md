# cour : **inline && block elements**

## 1. **Introduction:**


En HTML, les éléments peuvent être divisés en deux types principaux : les éléments en ligne (inline elements) et les éléments en bloc (block-level elements). La distinction entre ces deux types réside dans la manière dont ils sont rendus dans la structure de la page et comment ils interagissent les uns avec les autres.

1. **Éléments en ligne (Inline Elements) :**
   - Les éléments en ligne ne commencent pas sur une nouvelle ligne et ne prennent que l'espace nécessaire à leur contenu.
   - Ils ne forment pas de rupture de ligne, ce qui signifie que plusieurs éléments en ligne peuvent coexister sur la même ligne.
   - Exemples d'éléments en ligne : `<span>`, `<a>`, `<strong>`, `<em>`, `<img>`, `<br>`, `<code>`, etc.

   Exemple :
   ```html
   <p>Ceci est un texte <strong>important</strong> avec un <a href="#">lien</a>.</p>
   ```

2. **Éléments en bloc (Block-level Elements) :**
   - Les éléments en bloc commencent généralement sur une nouvelle ligne et occupent toute la largeur disponible de leur conteneur.
   - Ils forment une rupture de ligne avant et après eux, créant ainsi des « blocs » distincts dans la structure de la page.
   - Exemples d'éléments en bloc : `<div>`, `<p>`, `<h1>` à `<h6>`, `<ul>`, `<ol>`, `<li>`, `<table>`, etc.

   Exemple :
   ```html
   <div>
       <h1>Titre</h1>
       <p>Ceci est un paragraphe à l'intérieur d'un élément en bloc.</p>
   </div>
   ```

Il est important de comprendre ces différences pour bien structurer votre page web. Vous pouvez également rencontrer des éléments qui ont un comportement mixte, appelés éléments en ligne-bloc (inline-block elements), qui combinent certaines caractéristiques des deux types.


## 2. **``div:``**

>L'élément `<div>` en HTML est un élément de division qui est couramment utilisé pour regrouper d'autres éléments HTML afin de créer une structure et d'appliquer des styles CSS. Le nom "div" est une abréviation de "division". C'est un élément en bloc, ce qui signifie qu'il commence généralement sur une nouvelle ligne et occupe toute la largeur disponible de son conteneur.

- **Voici un exemple simple d'utilisation de l'élément `<div>` pour regrouper du contenu HTML :**

```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Exemple avec div</title>
    <style>
        /* Exemple de style CSS appliqué à la div */
        .conteneur {
            background-color: #f0f0f0;
            padding: 10px;
            border: 1px solid #ccc;
        }
    </style>
</head>
<body>

<!-- Utilisation de l'élément div -->
<div class="conteneur">
    <h1>Titre de la page</h1>
    <p>Ceci est un paragraphe à l'intérieur de la div.</p>
    <ul>
        <li>Élément de liste 1</li>
        <li>Élément de liste 2</li>
        <li>Élément de liste 3</li>
    </ul>
</div>

</body>
</html>
```

Dans cet exemple, la `<div>` a une classe appelée "conteneur", et des styles CSS sont appliqués à cette classe pour définir un fond de couleur, une marge intérieure (padding), et une bordure.

L'utilisation de `<div>` est fréquente pour structurer une page web de manière modulaire, en regroupant des sections de contenu et en facilitant l'application de styles ou la manipulation avec JavaScript.


## 3. **``span:``**

>L'élément `<span>` en HTML est un élément en ligne utilisé pour regrouper du texte ou d'autres éléments en ligne dans un document HTML, sans ajouter de nouvelle ligne. Il est souvent utilisé pour appliquer des styles, attributs ou événements spécifiques à une partie spécifique du texte.

- **Voici un exemple simple d'utilisation de l'élément `<span>` :**

```html
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Exemple avec span</title>
    <style>
        /* Exemple de style CSS appliqué à la span */
        .highlight {
            color: red;
            font-weight: bold;
        }
    </style>
</head>
<body>

<p>Ceci est un texte normal avec <span class="highlight">une partie mise en évidence</span>.</p>

</body>
</html>
```

Dans cet exemple, la balise `<span>` est utilisée avec la classe "highlight", et cette classe est ensuite stylée avec du CSS pour changer la couleur du texte en rouge et le rendre en gras.

L'élément `<span>` n'a généralement pas d'effet visible par défaut, mais il offre une structure de regroupement utile pour appliquer des styles ou des scripts à des parties spécifiques du texte. Il est souvent utilisé en conjonction avec des feuilles de style (CSS) ou du JavaScript pour manipuler dynamiquement le contenu.