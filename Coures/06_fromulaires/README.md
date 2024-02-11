# cour : **formulaires en HTML**


## 1. **Introduction:** 

>``Les formulaires`` en HTML constituent un élément essentiel dans le développement web, permettant aux utilisateurs d'interagir avec les pages en saisissant, envoyant et recevant des données. Un formulaire est un moyen interactif de collecter des informations auprès des visiteurs d'un site web. Que ce soit pour recueillir des commentaires, traiter des transactions en ligne, ou permettre aux utilisateurs de s'inscrire, les formulaires jouent un rôle crucial dans l'expérience utilisateur.

- ``widget`` en HTML fait référence à un élément d'interface utilisateur interactif qui est intégré dans une page web pour permettre aux utilisateurs d'effectuer des actions ou de fournir des informations.

- un formulaire en HTML est composé d'un ou plusieurs widgets, également appelés éléments de formulaire. Ces widgets sont des balises HTML spécifiques qui permettent aux utilisateurs d'entrer et de soumettre des données. 

- En HTML, les formulaires sont créés en utilisant la balise `<form>`, qui englobe divers éléments tels que les champs de texte, les cases à cocher, les boutons radio, les menus déroulants, et bien d'autres encore. Ces éléments sont définis à l'intérieur du formulaire à l'aide de balises spécifiques telles que `<input>`, `<textarea>`, `<select>`, etc.

- Chaque élément du formulaire peut être configuré avec des attributs pour définir son type, sa taille, ses options, et d'autres propriétés. De plus, les formulaires peuvent être envoyés à un serveur pour traitement en utilisant la méthode POST ou GET, permettant ainsi de traiter les données soumises côté serveur.


L'interaction entre les utilisateurs et les sites web est grandement facilitée par l'utilisation judicieuse des formulaires en HTML, offrant une expérience utilisateur interactive et dynamique. Dans cette introduction, nous explorerons les différents éléments de formulaire en HTML, ainsi que les attributs associés, pour comprendre comment créer des formulaires efficaces et conviviaux sur le web.


## 2. **L'élément `<form>` en HTML :**


- **Description :**

    L'élément `<form>` est utilisé pour créer un formulaire interactif sur une page web. Il englobe différents types d'éléments de formulaire tels que des champs de texte, des boutons, des cases à cocher, des listes déroulantes, etc. Cet élément définit la structure du formulaire et spécifie comment les données saisies par l'utilisateur doivent être traitées.


- **Syntaxe :**

    ```html
    <form action="URL_du_traitement" method="post|get" [autres attributs]>
        <!-- Éléments de formulaire vont ici -->
    </form>
    ```

- **Exemple :**
    ```html
    <form action="/traitement-du-formulaire" method="post">
        <label for="nom">Nom :</label>
        <input type="text" id="nom" name="nom" required>

        <label for="email">E-mail :</label>
        <input type="email" id="email" name="email" required>

        <input type="submit" value="Envoyer">
    </form>
    ```

- **Attributs :**

    1. **`action` :**
        - **Description :** Spécifie l'URL ou l'emplacement vers lequel les données du formulaire seront envoyées pour traitement côté serveur.
        - **Syntaxe :** `action="URL_du_traitement"`
        - **Exemple :** `action="/traitement-du-formulaire"`

    2. **`method` :**
        - **Description :** Indique la méthode HTTP à utiliser lors de l'envoi des données du formulaire. Les deux valeurs les plus courantes sont "post" et "get".
        - **Syntaxe :** `method="post|get"`
        - **Exemple :** `method="post"`



## 3. ***Widget `<input>` en HTML :**

### 3.1 **Introduction**


- **Description :**

    L'élément `<input>` est l'un des widgets les plus polyvalents en HTML, permettant la création de divers types de champs de saisie dans un formulaire. Il peut être utilisé pour collecter des informations telles que du texte, des mots de passe, des adresses e-mail, des cases à cocher, des boutons radio, etc.

- **Syntaxe générale :**

    ```html
    <input type="type_de_champ" name="
    " value="valeur_par_défaut" [autres_attributs]>
    ```
 
    - **`<input>` :** C'est la balise HTML qui crée un champ de saisie dans un formulaire.

    - **`type="type_de_champ"` :** Cet attribut `type` spécifie le type de champ de saisie que vous souhaitez créer. Il peut prendre différentes valeurs selon le type de données que vous souhaitez collecter. Par exemple, `text` pour une zone de texte, `password` pour un champ de mot de passe, `checkbox` pour une case à cocher, etc.

    - **`name="nom_du_champ"` :** L'attribut `name` associe un nom au champ de saisie. Ce nom est utilisé pour identifier le champ lors de la soumission du formulaire. Les données saisies dans ce champ seront associées à ce nom dans les données envoyées au serveur.

    - **`value="valeur_par_défaut"` :** L'attribut `value` définit la valeur initiale ou par défaut du champ de saisie. Cela peut être utile pour fournir une valeur pré-remplie ou suggérer une entrée à l'utilisateur.

    - **`[autres_attributs]` :** Cette partie de la syntaxe est facultative et représente d'autres attributs que vous pourriez utiliser en fonction des besoins spécifiques de votre champ de saisie. Certains exemples d'attributs supplémentaires incluent `placeholder` pour fournir un texte d'exemple, `autofocus` pour activer automatiquement le champ lors du chargement de la page, `required` pour rendre le champ obligatoire, et d'autres attributs spécifiques au type de champ.




### 3.2 **Liste des attributs :**

#### 3.2.1 **`type` :**

- **Description :** Spécifie le type de champ de saisie à créer (texte, mot de passe, case à cocher, bouton radio, etc.).


- **Exemple :**
    ```html
     <input type="text" name="username" value="JohnDoe">
    ```

- **listes des valeurs:**

Voici une description et un exemple pour chaque valeur possible de l'attribut `type` de l'élément `<input>` en HTML :

1. **`text` :**
   - **Description :** Crée une zone de texte pour la saisie de texte.
   - **Exemple :**
     ```html
     <input type="text" name="username" placeholder="Nom d'utilisateur">
     ```

2. **`button` :**
   - **Description :** Crée un simple bouton sans fonctionnalité spécifique.
   - **Exemple :**
     ```html
     <input type="button" value="Cliquez-moi">
     ```

3. **`checkbox` :**
   - **Description :** Crée une case à cocher permettant à l'utilisateur de sélectionner ou désélectionner une option.
   - **Exemple :**
     ```html
     <input type="checkbox" name="subscribe" id="subscribe"> <label for="subscribe">S'abonner</label>
     ```

4. **`color` :**
   - **Description :** Affiche une palette de couleurs pour la sélection d'une couleur.
   - **Exemple :**
     ```html
     <input type="color" name="background_color" value="#ff0000">
     ```

5. **`date` :**
   - **Description :** Permet de sélectionner une date dans un calendrier.
   - **Exemple :**
     ```html
     <input type="date" name="birthdate">
     ```

6. **`email` :**
   - **Description :** Crée une zone de texte conçue pour la saisie d'une adresse e-mail.
   - **Exemple :**
     ```html
     <input type="email" name="email" placeholder="Entrez votre e-mail">
     ```

7. **`file` :**
   - **Description :** Permet à l'utilisateur de sélectionner un fichier à envoyer avec le formulaire.
   - **Exemple :**
     ```html
     <input type="file" name="file_upload">
     ```

8. **`image` :**
   - **Description :** Crée un bouton d'image pour être utilisé dans un formulaire.
   - **Exemple :**
     ```html
     <input type="image" src="bouton-image.png" alt="Bouton image">
     ```

9. **`number` :**
   - **Description :** Permet la saisie d'un nombre.
   - **Exemple :**
     ```html
     <input type="number" name="quantity" min="1" max="10" value="1">
     ```

10. **`password` :**
    - **Description :** Crée une zone de texte où les caractères sont masqués, souvent utilisée pour la saisie de mots de passe.
    - **Exemple :**
      ```html
      <input type="password" name="password" placeholder="Mot de passe">
      ```

11. **`radio` :**
    - **Description :** Crée un bouton radio permettant à l'utilisateur de sélectionner une option parmi plusieurs.
    - **Exemple :**
      ```html
      <input type="radio" name="gender" value="male"> Homme
      <input type="radio" name="gender" value="female"> Femme
      ```

12. **`range` :**
    - **Description :** Permet à l'utilisateur de sélectionner une valeur numérique dans une plage spécifiée.
    - **Exemple :**
      ```html
      <input type="range" name="volume" min="0" max="100" value="50">
      ```

13. **`reset` :**
    - **Description :** Crée un bouton qui réinitialise tous les champs du formulaire à leurs valeurs par défaut.
    - **Exemple :**
      ```html
      <input type="reset" value="Effacer">
      ```

14. **`search` :**
    - **Description :** Crée une zone de texte pour la saisie de termes de recherche.
    - **Exemple :**
      ```html
      <input type="search" name="query" placeholder="Recherche...">
      ```

15. **`submit` :**
    - **Description :** Crée un bouton qui soumet le formulaire lorsque l'utilisateur le clique.
    - **Exemple :**
      ```html
      <input type="submit" value="Envoyer">
      ```

16. **`tel` :**
    - **Description :** Permet la saisie d'un numéro de téléphone.
    - **Exemple :**
      ```html
      <input type="tel" name="phone_number" placeholder="Numéro de téléphone">
      ```

17. **`time` :**
    - **Description :** Permet la saisie d'une heure.
    - **Exemple :**
      ```html
      <input type="time" name="meeting_time">
      ```

18. **`url` :**
    - **Description :** Crée une zone de texte conçue pour la saisie d'une URL.
    - **Exemple :**
      ```html
      <input type="url" name="website" placeholder="Entrez l'URL">
      ```

Chaque type d'attribut `type` a des fonctionnalités spécifiques qui répondent aux besoins de collecte de données spécifiques dans un formulaire HTML.



#### 3.2.2 **`name` :**

- **Description :** Associe un nom au champ, permettant de l'identifier lors de la soumission du formulaire.

- **Exemple :**
     ```html
     <input type="checkbox" name="subscribe" id="subscribe"> <label for="subscribe">S'abonner</label>
     ```

#### 3.2.3 **`value` :**

- **Description :** Définit la valeur initiale ou par défaut du champ.

- **Exemple :**
     ```html
     <input type="text" name="firstname" value="John">
     ```

#### 3.2.4 **`placeholder` :**

- **Description :** Fournit un texte d'exemple ou une suggestion pour indiquer à l'utilisateur le type d'information attendue.


- **Exemple :**
     ```html
     <input type="email" name="email" placeholder="Entrez votre adresse e-mail">
     ```

#### 3.2.5 **`autofocus` :**
   
- **Description :** Indique que le champ doit être automatiquement activé lors que la page se charge.

- **Exemple :**
     ```html
     <input type="text" name="username" autofocus>
     ```

#### 3.2.6 **`required` :**
   
- **Description :** Spécifie que le champ doit être rempli par l'utilisateur avant de soumettre le formulaire.

- **Exemple :**
     ```html
     <input type="text" name="username" required>
     ```

#### 3.2.7 **`disabled` :**

- **Description :** Désactive le champ, empêchant l'utilisateur de l'éditer ou de l'activer.

- **Exemple :**
     ```html
     <input type="text" name="city" disabled>
     ```

#### 3.2.8 **Attribut `readonly` :**

- **Description :** L'attribut `readonly` est utilisé pour rendre un champ de saisie en lecture seule, ce qui signifie que l'utilisateur peut voir le contenu du champ, mais il ne peut pas le modifier ni y entrer de nouvelles données.

- **Exemple :**
  ```html
  <input type="text" name="username" value="JohnDoe" readonly>
  ```

**Attribut `tabindex` :**

- **Description :** L'attribut `tabindex` spécifie l'ordre de tabulation des éléments sur une page. Il indique à quel indice l'élément doit être placé dans la séquence de tabulation lorsqu'un utilisateur navigue à travers les éléments à l'aide de la touche Tab.

- **Exemple :**
  ```html
  <input type="text" name="firstname" tabindex="1">
  <input type="text" name="lastname" tabindex="2">
  <input type="submit" value="Envoyer" tabindex="3">
  ```



## 4. **Widget `<textarea>` en HTML :**

- **Description :**
    L'élément `<textarea>` en HTML est utilisé pour créer une zone de texte multi-lignes, permettant aux utilisateurs de saisir du texte sur plusieurs lignes.

- **Syntaxe :**

    ```html
    <textarea name="nom_du_champ" rows="nombre_de_lignes" cols="nombre_de_colonnes" [autres_attributs]>Contenu par défaut</textarea>
    ```

- **Exemple :**
    ```html
    <textarea name="message" rows="4" cols="50" placeholder="Saisissez votre message ici..."></textarea>
    ```

- **Attributs couramment utilisés :**

    1. **`name` :**
        - **Description :** Associe un nom à la zone de texte, identifiant ainsi le champ lors de la soumission du formulaire.
        - **Exemple :** `name="message"`

    2. **`rows` :**
        - **Description :** Spécifie le nombre visible de lignes de texte dans la zone de texte.
        - **Exemple :** `rows="4"`

    3. **`cols` :**
        - **Description :** Spécifie le nombre de caractères visibles par ligne dans la zone de texte.
        - **Exemple :** `cols="50"`

    4. **`placeholder` :**
        - **Description :** Fournit un texte d'exemple ou une suggestion pour indiquer à l'utilisateur le type d'information attendue.
        - **Exemple :** `placeholder="Saisissez votre message ici..."`

    5. **`readonly` :**
        - **Description :** Rend la zone de texte en lecture seule, empêchant l'utilisateur de modifier le contenu.
        - **Exemple :** `readonly`

La balise `<textarea>` est particulièrement utile lorsque vous avez besoin de collecter des informations de texte plus longues, comme des commentaires ou des descriptions, par opposition au champ de saisie `<input type="text">` qui est adapté pour des entrées de texte plus courtes.



## 5. **L'élément `<label>`:**

- **Description :**
    L'élément `<label>` en HTML est utilisé pour associer un libellé à un élément de formulaire, tel qu'un champ de saisie ou une case à cocher. Cela améliore l'accessibilité et la convivialité du formulaire en permettant aux utilisateurs de cliquer sur le libellé pour activer le champ associé.

- **Syntaxe :**
    ```html
    <label for="id_de_l_element">Texte du libellé</label>
    ```

- **Exemple avec un champ de saisie :**
    ```html
    <label for="username">Nom d'utilisateur :</label>
    <input type="text" id="username" name="username">
    ```

    Dans cet exemple, le libellé "Nom d'utilisateur :" est associé au champ de saisie avec l'attribut `id="username"` et l'attribut `for` dans la balise `<label>`.

- **Exemple avec une case à cocher :**
    ```html
    <label for="subscribe">S'abonner :</label>
    <input type="checkbox" id="subscribe" name="subscribe">
    ```

    Ici, le libellé "S'abonner :" est associé à la case à cocher avec l'attribut `id="subscribe"` et l'attribut `for` dans la balise `<label>`.


- L'utilisation de l'élément `<label>` présente plusieurs avantages :

    1. **Amélioration de l'accessibilité :** Les utilisateurs peuvent cliquer sur le libellé pour activer le champ associé, ce qui est particulièrement utile pour les personnes utilisant des lecteurs d'écran.

    2. **Meilleure convivialité :** Le libellé rend le formulaire plus convivial en fournissant des indications claires sur la signification du champ.

    3. **Stylisation facilitée :** L'élément `<label>` permet de styliser le libellé indépendamment du champ, offrant ainsi plus de flexibilité en matière de conception.

    En résumé, l'élément `<label>` est un élément important pour améliorer l'expérience utilisateur et l'accessibilité des formulaires HTML.



## 6. **L'élément `<button>`:**

- **Description :**
    L'élément `<button>` en HTML est utilisé pour créer un bouton interactif dans une page web. Ce bouton peut être utilisé pour déclencher des actions JavaScript ou pour soumettre un formulaire. L'élément `<button>` offre une flexibilité en termes de contenu, car il peut contenir du texte, des images, ou même d'autres éléments HTML.


- **Syntaxe :**
    ```html
    <button type="type_de_bouton" [autres_attributs]>Contenu du bouton</button>
    ```

- **Exemple :**
    ```html
    <button type="button" onclick="alert('Clic effectué !')">Cliquez-moi</button>
    ```


- **Attributs couramment utilisés :**

    1. **`type` :**
        - **Description :** Spécifie le type de bouton. Les valeurs courantes sont "button" (par défaut), "submit" pour soumettre un formulaire, et "reset" pour réinitialiser un formulaire.
        - **Exemple :** `type="button"`

    2. **`name` :**
        - **Description :** Associe un nom au bouton, généralement utilisé lors de la soumission d'un formulaire.
        - **Exemple :** `name="submit_button"`

    3. **`value` :**
        - **Description :** Définit la valeur initiale du bouton, utilisée lors de la soumission d'un formulaire.
        - **Exemple :** `value="Envoyer"`

    4. **`disabled` :**
        - **Description :** Désactive le bouton, empêchant l'utilisateur de l'activer.
        - **Exemple :** `disabled`

    5. **`onclick` :**
        - **Description :** Définit une action JavaScript à exécuter lorsque le bouton est cliqué.
        - **Exemple :** `onclick="alert('Clic effectué !')"`

    6. **`autofocus` :**
        - **Description :** Indique que le bouton doit être automatiquement activé lors que la page se charge.
        - **Exemple :** `autofocus`

- **Exemple avec un formulaire :**
    ```html
    <form action="/traitement-du-formulaire" method="post">
        <input type="text" name="username" placeholder="Nom d'utilisateur">
        <input type="password" name="password" placeholder="Mot de passe">
        <button type="submit">Se connecter</button>
    </form>
    ```

    Dans cet exemple, le bouton est utilisé pour soumettre le formulaire vers l'URL "/traitement-du-formulaire" en utilisant la méthode "post". Vous pouvez personnaliser le contenu et le comportement du bouton en fonction de vos besoins spécifiques.



## 7. **L'élément `<select>`:**

- **Description :**
    L'élément `<select>` en HTML est utilisé pour créer une liste déroulante (menu déroulant) dans un formulaire. Cela permet aux utilisateurs de sélectionner une option parmi plusieurs. L'élément `<select>` est souvent associé à des balises `<option>` qui définissent les différentes options disponibles dans la liste déroulante.

- **Syntaxe de base :**
    ```html
    <select name="nom_du_champ" [autres_attributs]>
        <option value="valeur_option1">Option 1</option>
        <option value="valeur_option2">Option 2</option>
        <!-- Ajoutez d'autres options si nécessaire -->
    </select>
    ```

- **Exemple simple :**
    ```html
    <select name="pays">
        <option value="france">France</option>
        <option value="espagne">Espagne</option>
        <option value="italie">Italie</option>
    </select>
    ```

- **Attributs couramment utilisés :**

1. **`name` :**
   - **Description :** Associe un nom à la liste déroulante, permettant de l'identifier lors de la soumission du formulaire.
   - **Exemple :** `name="pays"`

2. **`size` :**
   - **Description :** Spécifie le nombre visible d'options dans la liste déroulante lorsque celle-ci est dépliée.
   - **Exemple :** `size="3"`

3. **`multiple` :**
   - **Description :** Permet à l'utilisateur de sélectionner plusieurs options en même temps. Ajoutez cet attribut pour créer une liste déroulante à sélection multiple.
   - **Exemple :** `multiple`

4. **`disabled` :**
   - **Description :** Désactive la liste déroulante, empêchant l'utilisateur de la sélectionner.
   - **Exemple :** `disabled`

5. **`autofocus` :**
   - **Description :** Indique que la liste déroulante doit être automatiquement activée lors que la page se charge.
   - **Exemple :** `autofocus`

6. **`selected`:**
    - **Description :** L'attribut `selected` est utilisé pour définir une option pré-sélectionnée dans une liste déroulante. 

    - **Exemple :**
        ```html
        <select name="pays">
            <option value="france">France</option>
            <option value="espagne" selected>Espagne</option>
            <option value="italie">Italie</option>
        </select>
        ```


7. **`optgroup`:**
    - **Description :** L'élément `<optgroup>` est utilisé pour regrouper plusieurs options au sein d'une liste déroulante. Cela permet de structurer les options en catégories ou sections.

    - **Exemple :**
        ```html
        <select name="fruits">
            <optgroup label="Fruits rouges">
                <option value="fraise">Fraise</option>
                <option value="cerise">Cerise</option>
                <option value="framboise">Framboise</option>
            </optgroup>
            <optgroup label="Fruits jaunes">
                <option value="banane">Banane</option>
                <option value="ananas">Ananas</option>
                <option value="mangue">Mangue</option>
            </optgroup>
        </select>
        ```



L'élément `<select>` est essentiel pour créer des formulaires interactifs avec des options de sélection, offrant aux utilisateurs une interface conviviale pour choisir parmi différentes alternatives.



## 8. **L'élément `fieldset`:**

- **Description :**
    L'attribut `fieldset` en HTML est utilisé pour regrouper des éléments de formulaire associés au sein d'une boîte entourée d'une bordure. Il est souvent utilisé en conjonction avec l'élément `legend` pour fournir un titre ou une légende descriptif pour le groupe de champs associé.


- **Syntaxe :**
    ```html
    <fieldset>
        <legend>Titre du groupe</legend>
        <!-- Les éléments de formulaire vont ici -->
    </fieldset>
    ```

- **Exemple :**
    ```html
    <fieldset>
        <legend>Informations personnelles</legend>
        <label for="nom">Nom :</label>
        <input type="text" id="nom" name="nom">

        <label for="prenom">Prénom :</label>
        <input type="text" id="prenom" name="prenom">

        <!-- Ajoutez d'autres champs de formulaire si nécessaire -->
    </fieldset>
    ```

    Dans cet exemple, les champs de formulaire associés aux informations personnelles sont regroupés dans un `fieldset` avec la légende "Informations personnelles". L'utilisation de `fieldset` peut rendre la structure du formulaire plus claire et faciliter la compréhension des utilisateurs, en particulier lorsque le formulaire est complexe et comporte plusieurs sections distinctes.

- **Attributs couramment utilisés avec `fieldset` :**

1. **`disabled` :**
   - **Description :** Désactive tous les éléments de formulaire à l'intérieur du `fieldset`, empêchant l'utilisateur d'interagir avec eux.
   - **Exemple :** `<fieldset disabled>...</fieldset>`

2. **`form` :**
   - **Description :** Indique le formulaire auquel le `fieldset` appartient, en utilisant l'ID du formulaire.
   - **Exemple :** `<fieldset form="monFormulaire">...</fieldset>`

L'utilisation de `fieldset` améliore la séparation logique des sections d'un formulaire et offre une meilleure structure visuelle pour les utilisateurs. Il est souvent utilisé pour améliorer l'accessibilité et l'expérience utilisateur dans les formulaires complexes.



## 9. **l'élément `<progress>` et l'élément `<meter>`:**


### 9.1 **L'élément `<progress>` :**


>L'élément `<progress>` est utilisé pour créer une barre de progression dans une page web, généralement pour indiquer la progression d'une tâche en cours.


- **Syntaxe :**
    ```html
    <progress value="valeur_actuelle" max="valeur_maximale">Progression</progress>
    ```

- **Exemple :**
    ```html
    <progress value="50" max="100">50%</progress>
    ```

    Dans cet exemple, la barre de progression est à 50% de sa valeur maximale.

- **Attributs couramment utilisés :**
    1. **`value` :**
        - **Description :** Spécifie la valeur actuelle de la progression.
        - **Exemple :** `<progress value="30" max="100">30%</progress>`

    2. **`max` :**
        - **Description :** Définit la valeur maximale possible de la progression.
        - **Exemple :** `<progress value="20" max="50">40%</progress>`


### 9.2 **l'élément `<meter>`:**

>l'élément `<meter>`, il est utilisé pour représenter une mesure scalaire dans une plage connue ou un ensemble de mesures. Il peut être utilisé pour indiquer des valeurs comme la capacité d'une batterie, la satisfaction d'un client, etc.


- **L'élément `<meter>` :**
    ```html
    <meter value="valeur_actuelle" min="valeur_minimale" max="valeur_maximale">Métrique</meter>
    ```

- **Exemple :**
    ```html
    <meter value="75" min="0" max="100">75%</meter>
    ```

    Dans cet exemple, le `<meter>` affiche une métrique de 75% dans la plage de 0 à 100.

- **Attributs couramment utilisés :**
    1. **`value` :**
        - **Description :** Spécifie la valeur actuelle de la métrique.
        - **Exemple :** `<meter value="50" min="0" max="100">50%</meter>`

    2. **`min` :**
        - **Description :** Définit la valeur minimale possible de la métrique.
        - **Exemple :** `<meter value="25" min="0" max="100">25%</meter>`

    3. **`max` :**
        - **Description :** Définit la valeur maximale possible de la métrique.
        - **Exemple :** `<meter value="80" min="0" max="100">80%</meter>`

Les éléments `<progress>` et `<meter>` sont utiles pour afficher visuellement la progression ou la mesure d'une tâche ou d'une métrique dans une page web.





