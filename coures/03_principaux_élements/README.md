# cour 03 : **``les principaux élements HTML``**

## 1. **les principaux élements HTML:**

1. **`<h1> à <h6>` Titres HTML :**

   - **Description :** Ces balises sont utilisées pour définir les titres et sous-titres d'une page HTML. `<h1>` est le titre le plus important, `<h6>` est le moins important.

   - **Utilisation :** 
     ```html
     <h1>Titre Principal</h1>
     <h2>Sous-Titre</h2>
     <h3>Autre Niveau de Titre</h3>
     ```

2. **`<p>` - Paragraphe :**

   - **Description :** Cette balise est utilisée pour définir un paragraphe de texte.

   - **Utilisation :**
     ```html
     <p>Ceci est un paragraphe de texte.</p>
     ```

3. **`<em>` - Texte en italique :**

   - **Description :** Cette balise est utilisée pour mettre en évidence du texte et lui donner une emphase en l'affichant en italique.

   - **Utilisation :**
     ```html
     <p>Ceci est du texte <em>en italique</em>.</p>
     ```

4. **`<strong>` - Texte en gras :**

   - **Description :** Cette balise est utilisée pour indiquer que le texte qu'elle enveloppe doit être affiché en gras.

   - **Utilisation :**
     ```html
     <p>Ceci est du texte <strong>en gras</strong>.</p>
     ```

5. **`<br>` - Saut de ligne :**

   - **Description :** Cette balise est utilisée pour insérer un saut de ligne à l'intérieur du texte.

   - **Utilisation :**
     ```html
     <p>Ceci est une phrase.<br>Et voici une nouvelle ligne.</p>
     ```

6. **`<hr>` - Ligne horizontale :**

   - **Description :** Cette balise est utilisée pour créer une ligne horizontale, souvent utilisée pour séparer des sections de contenu.

   - **Utilisation :**
     ```html
     <p>Contenu avant la ligne horizontale</p>
     <hr>
     <p>Contenu après la ligne horizontale</p>
     ```

7. **`<del>` - Texte barré :**

   - **Description :** Cette balise est utilisée pour indiquer que le texte qu'elle enveloppe a été supprimé ou n'est plus valide.

   - **Utilisation :**
     ```html
     <p>Ce texte est <del>barré</del> supprimé.</p>
    
     ```

    
## 2. **les commentaires En HTML :**


- **Définition:**
    
    - les commentaires sont utilisés pour inclure des annotations ou des notes dans le code source, et ils ne sont pas affichés dans le navigateur lorsqu'une page est rendue. 
    
    - Les commentaires sont utiles pour documenter le code, expliquer des sections spécifiques, ou désactiver temporairement des parties du code. 
    
    - Les commentaires HTML commencent par `<!--` et se terminent par `-->`. Tout ce qui se trouve entre ces balises est considéré comme un commentaire et est ignoré lors de l'affichage de la page dans un navigateur.

- **Commentaire sur une ligne :**
```html
<!-- Ceci est un commentaire sur une ligne -->
```


- **Commentaire sur plusieurs lignes :**

```html
<!--
  Ceci est un commentaire
  sur plusieurs lignes.
-->
```



- **Exemple d'utilisation dans un code HTML :**

```html
<!DOCTYPE html>
<html>
<head>
  <title>Ma Page Web</title>
  <!-- Inclure une feuille de style externe -->
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <h1>Bienvenue sur ma page!</h1>
  <p>Ceci est un paragraphe de texte.</p>
  <!-- L'image suivante est optionnelle -->
  <img src="image.jpg" alt="Description de l'image">
</body>
</html>
```


