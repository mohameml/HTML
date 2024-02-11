# cour 01 : Introduction à HTML

## 1. **Introduction à HTML:**

- **HTML**, acronyme de **HyperText Markup Language**, est le langage de balisage standard utilisé pour créer et concevoir des pages web. 

- Il s'agit d'un langage essentiel pour le développement web, permettant de structurer le contenu d'une page de manière logique et compréhensible pour les navigateurs web.



## 2. **Structure de base d'un document HTML:**

- voici la structure minimale d'une page HTML :

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Titre de la page</title>
  </head>
  <body>
    <!-- Le contenu de la page va ici -->
  </body>
</html>
```


1. `<!DOCTYPE html>` : 
  
  - Cette déclaration, appelée déclaration ``DOCTYPE``, indique au navigateur quelle version de HTML la page utilise. Dans ce cas, `<!DOCTYPE html>` indique que la page utilise la version ``HTML5``.

2. `<html>` : La balise `<html>` est la racine de tout document HTML. Elle englobe l'ensemble du contenu de la page.

3. `<head>` : 
  
  - La section `<head>` contient des informations sur le document, telles que le titre de la page, les liens vers des feuilles de style (CSS), les scripts JavaScript, les méta-informations, etc. 
  
  - Ces informations ne sont généralement pas affichées directement sur la page, mais elles jouent un rôle crucial dans la configuration et la description de la page.

  - `<title>` : La balise `<title>` est utilisée pour définir le titre de la page, qui apparaît dans l'onglet du navigateur ou dans la barre de titre de la fenêtre du navigateur.



4. `<body>` : 

  - La section `<body>` contient tout le contenu réel de la page, tel que le texte, les images, les liens, les formulaires, etc. C'est la partie visible de la page web.




## 3. **les élément HTML && les balises HTML :**

- **Définition:les élément HTML**
  
  - **Un élément HTML:** est un composant de base dans la construction d'une page web à l'aide du langage de balisage HTML. 
  
  - **Les éléments HTML:** sont les éléments de base qui permettent de structurer et de présenter le contenu d'une page web de manière cohérente et sémantique. 

  - Chaque élément HTML est défini par :

    - une ou plusieurs **balises** 
    
    - des **attributs** 
    
    - et d'autres éléments HTML : **`imbrication`**. 

    -  et peut contenir du texte : **le contenu**
    

  

- **Définition les balise HTML:**

  - **Une balise HTML:** est un ensemble de caractères délimités par des chevrons (``<`` et ``>``) qui déclare et structure un élément HTML. 
  
  - Elle peut être une balise d'ouverture, une balise de fermeture, ou une balise autofermante, selon le type d'élément qu'elle représente.

  
  - **Balise d'ouverture**: La balise d'ouverture marque le début d'un élément HTML et spécifie le type de l'élément. Elle est constituée du nom de la balise entouré par des chevrons. Par exemple, `<p>` est une balise d'ouverture qui déclare le début d'un paragraphe.

  
  - **Balise de fermeture**: La balise de fermeture marque la fin d'un élément HTML. Elle ressemble à la balise d'ouverture, mais avec une barre oblique (``/``) avant le nom de la balise. Par exemple, `</p>` est une balise de fermeture qui déclare la fin du paragraphe ouvert par `<p>`.

  
  - **Balise autofermante**: Certains éléments HTML n'ont pas de contenu à l'intérieur et se ferment automatiquement. Ils sont écrits sous la forme d'une balise unique autofermante. Par exemple, `<img src="image.jpg" alt="Description">` est une balise autofermante qui insère une image.



- **une structure générale d'un élément HTML :**

  ```html
  <balise attribut="valeur">Contenu de l'élément</balise>
  ```

  - **Balise**: Il s'agit du nom de l'élément, par exemple, `<p>` pour un paragraphe, `<h1>` pour un titre de niveau 1, `<a>` pour un lien, etc.

  - **Attribut**: Les attributs fournissent des informations supplémentaires sur l'élément et sont spécifiés dans la balise d'ouverture. Par exemple, dans `<a href="https://www.example.com">`, `href` est un attribut qui spécifie l'URL vers laquelle le lien pointe.

  - **Contenu de l'élément**: C'est le texte ou d'autres éléments HTML inclus entre la balise d'ouverture et la balise de fermeture.


- **Exemple avec ``un paragraphe : <p>`` :**

  ```html
  <p>Ceci est un paragraphe d'exemple.</p>
  ```

  Dans cet exemple, `<p>` est la balise d'ouverture, `</p>` est la balise de fermeture, et "Ceci est un paragraphe d'exemple." est le contenu de l'élément.




## 4. **principe de L'imbrication en HTML:**

- **L'imbrication en HTML:** fait référence à la pratique de placer un élément HTML à l'intérieur d'un autre. 

- Cette technique est essentielle pour définir la structure et l'organisation du contenu d'une page web de manière logique. 

- Voici les principes de base de l'imbrication en HTML :

1. **Ouverture et fermeture des balises :** 
  
  - Chaque balise ouverte doit être correctement fermée. Par exemple, si vous ouvrez une balise `<div>`, assurez-vous de la fermer avec `</div>`. L'imbrication incorrecte ou l'absence de fermeture peuvent entraîner des erreurs d'interprétation du code HTML par le navigateur.

    ```html
    <!-- Correct -->
    <div>
        <p>Contenu de la div</p>
    </div>

    <!-- Incorrect (imbrication non fermée) -->
    <div>
        <p>Contenu de la div</p>
    
    ```

2. **Imbrication hiérarchique :** 

  - Les éléments doivent être correctement hiérarchisés. Cela signifie que vous devez respecter l'ordre naturel des balises dans la structure HTML. Par exemple, les balises de titre `<h1>` à `<h6>` devraient normalement être à l'intérieur de la balise `<body>`, et non directement dans la balise `<head>`.

    ```html
    <!-- Correct -->
    <body>
        <h1>Titre principal</h1>
        <p>Contenu de la page</p>
    </body>

    <!-- Incorrect (h1 directement dans head) -->
    <head>
        <h1>Titre principal</h1>
    </head>
    ```

3. **Nesting logique :** 
  
  - Placez les balises de manière logique en fonction de la signification sémantique de votre contenu. Par exemple, un paragraphe `<p>` peut contenir du texte, mais il n'est pas logique de placer un paragraphe à l'intérieur d'un en-tête `<h1>`.

    ```html
    <!-- Correct -->
    <article>
        <h2>Titre de l'article</h2>
        <p>Contenu de l'article</p>
    </article>

    <!-- Incorrect (p à l'intérieur de h2) -->
    <h2>Titre de l'article<p>Contenu de l'article</p></h2>
    ```

4. **Éviter les imbrications excessives :** 

  - Bien que l'imbrication soit nécessaire, une imbrication excessive peut rendre le code difficile à lire et à comprendre. Essayez de maintenir une structure simple et claire.

    ```html
    <!-- Correct -->
    <div>
        <p>Contenu</p>
    </div>

    <!-- Éviter (imbrication excessive) -->
    <div>
        <div>
            <div>
                <p>Contenu</p>
            </div>
        </div>
    </div>
    ```








