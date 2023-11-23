# cour 09 : **les métadonnées:**


## 1. **Définition:**

- les métadonnées (meta données) sont des informations sur les données elles-mêmes. Les balises `<meta>` sont utilisées pour fournir des métadonnées dans le code source d'une page HTML. Ces informations ne sont généralement pas affichées à l'utilisateur, mais elles fournissent des informations importantes pour les navigateurs web, les moteurs de recherche et d'autres applications.

Voici quelques-uns des attributs couramment utilisés avec la balise `<meta>` :

1. **`charset` :**
   - **Description :** Spécifie le jeu de caractères utilisé dans le document.
   - **Exemple :** `<meta charset="UTF-8">`

2. **`name` et `content` :**
   - **Description :** Souvent utilisés ensemble pour fournir des informations spécifiques. Par exemple, `<meta name="description" content="Une brève description de la page.">`.

3. **`http-equiv` :**
   - **Description :** Fournit un équivalent HTTP pour les entêtes HTTP. Par exemple, `<meta http-equiv="refresh" content="30">` pour actualiser automatiquement la page toutes les 30 secondes.

4. **`viewport` :**
   - **Description :** Utilisé pour contrôler le dimensionnement et l'échelle de la vue sur les appareils mobiles.
   - **Exemple :** `<meta name="viewport" content="width=device-width, initial-scale=1.0">`

5. **`robots` :**
   - **Description :** Contrôle le comportement des robots des moteurs de recherche.
   - **Exemple :** `<meta name="robots" content="index, follow">` pour autoriser l'indexation et le suivi par les moteurs de recherche.

6. **`author` :**
   - **Description :** Indique l'auteur de la page.
   - **Exemple :** `<meta name="author" content="Nom de l'auteur">`

7. **`viewport` :**
   - **Description :** Utilisé pour définir la largeur visible de la fenêtre d'affichage.
   - **Exemple :** `<meta name="viewport" content="width=device-width, initial-scale=1.0">`

8. **`keywords` :**
   - **Description :** Fournit une liste de mots-clés associés à la page.
   - **Exemple :** `<meta name="keywords" content="mot-clé1, mot-clé2, mot-clé3">`

Ces balises `<meta>` permettent aux développeurs web de fournir des informations importantes pour le rendu de la page, l'indexation par les moteurs de recherche, et d'autres aspects qui peuvent influencer l'expérience de l'utilisateur et la manière dont la page est traitée par les différents logiciels.