# cour 02 : **`les attributs`**



## 1. **Définition:**


- **Un attribut** en HTML est :
    
    - une caractéristique supplémentaire spécifiée dans une balise pour fournir des informations ou des instructions supplémentaires sur l'élément. 
    
    - Les attributs sont inclus dans la balise en utilisant la syntaxe `nom="valeur"`.



## 2. **Règles à respecter pour définir un attribut :**



- **Espace avec la Balise :** 
    
    - Les attributs sont spécifiés à l'intérieur de la balise de l'élément auquel ils sont associés . 
    
    - Il n'y a pas d'espace entre le nom de l'attribut, le signe égal (=) et la valeur de l'attribut. Par exemple : 
        
        `<img src="image.jpg" alt="Image de démonstration">`.

- **Nom de l'Attribut :** 
    
    - Il s'agit du nom qui identifie l'attribut spécifique que vous souhaitez utiliser. 
    
    - Par exemple, dans l'attribut `src="image.jpg"`, "src" est le nom de l'attribut.

- **Valeur de l'Attribut :** 
    
    - Il s'agit de la valeur assignée à l'attribut. La valeur est toujours placée entre guillemets (simples ou doubles). 
    
    - Dans l'exemple `src="image.jpg"`, "image.jpg" est la valeur de l'attribut "src".

- **Nom de l'Attribut en Minuscules :** 

    - Les noms d'attributs en HTML ne sont pas sensibles à la casse, mais il est une convention de les écrire en minuscules pour des raisons de cohérence et de lisibilité du code. Cependant, les valeurs peuvent être sensibles à la casse.




## 3. **QQ Attributs :**


1. **`lang` :**
   - **Description :** L'attribut `lang` spécifie la langue de l'élément.
   - **Exemple :** `<html lang="fr">`

2. **`href` :**
   - **Description :** L'attribut `href` spécifie l'URL de destination pour les liens hypertexte.
   - **Exemple :** `<a href="https://www.example.com">Visitez notre site web</a>`

3. **`src` :**
   - **Description :** L'attribut `src` spécifie la source (URL ou chemin local) de la ressource, généralement utilisé avec les balises `<img>`, `<script>`, et `<iframe>`.
   - **Exemple :** `<img src="image.jpg" alt="Description de l'image">`

4. **`width` :**
   - **Description :** L'attribut `width` spécifie la largeur de l'élément, généralement utilisé avec les balises `<img>` et `<iframe>`.
   - **Exemple :** `<img src="image.jpg" alt="Description de l'image" width="300">`

5. **`height` :**
   - **Description :** L'attribut `height` spécifie la hauteur de l'élément, généralement utilisé avec les balises `<img>` et `<iframe>`.
   - **Exemple :** `<img src="image.jpg" alt="Description de l'image" height="200">`

6. **`alt` :**
   - **Description :** L'attribut `alt` fournit un texte alternatif qui s'affiche si l'image ne peut pas être chargée. Il est également utilisé pour l'accessibilité.
   - **Exemple :** `<img src="image.jpg" alt="Description de l'image">`

7. **`style` :**
   - **Description :** L'attribut `style` permet d'appliquer des styles CSS en ligne à un élément.
   - **Exemple :** `<p style="color: blue; font-size: 16px;">Texte stylisé en bleu</p>`

8. **`title` :**
   - **Description :** L'attribut `title` fournit un texte descriptif qui apparaît généralement comme une info-bulle lorsque la souris survole l'élément.
   - **Exemple :** `<a href="https://www.example.com" title="Site Web">Visitez notre site web</a>`
