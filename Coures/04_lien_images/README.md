# cour 04 : **hyperliens et images :**


## 1. **``hyperliens:``**

### a. **Définition:**

- **Un hyperlien:**, est un élément interactif dans un document  (tel qu'une page Web) qui permet aux utilisateurs de naviguer vers un autre emplacement, que ce soit dans le même document ou vers un document différent. Les hyperliens sont la base de la navigation sur le Web.

- Les hyperliens sont généralement créés à l'aide de la balise HTML `<a>` . 
    

- Un hyperlien peut pointer vers diverses ressources, telles que d'autres pages Web, des fichiers, des images, des adresses électroniques, etc. 
    


- Lorsqu'un utilisateur clique sur un hyperlien, il est redirigé vers la destination spécifiée par l'attribut `href` (HyperReference) de la balise `<a>`.


### b.  **la balise ``<a>``:**


- **un hyperlien sé declare avce la balise :**

    ```html
    <a  herf="lien"> Text </a>
    ```
        
    - `href` : spécifie l'URL de la page vers laquelle le lien pointe.



### c. **les attributs de la balise  ``<a>``:**


- La balise `<a>` peut contenir plusieurs attributs pour spécifier diverses informations liées au lien. 


- Voici quelques-uns des attributs les plus couramment utilisés avec la balise `<a>` :

1. **`href` (HyperReference) :** 
    
    - Cet attribut spécifie l'URL de destination du lien. Il peut pointer vers une page Web, un fichier, une adresse e-mail, ou d'autres types de ressources.

   - Exemple :
    ```html
    <a href="https://www.example.com">Visitez Example.com</a>
    ```

2. **`target` :** 
    
    -  Cet attribut spécifie où ou comment ouvrir le lien. 
    
    - Les valeurs courantes sont :
    - `_blank` : Ouvre le lien dans une nouvelle fenêtre ou un nouvel onglet.
    - `_self` : Ouvre le lien dans la même fenêtre ou le même onglet (c'est la valeur par défaut).

   - Exemple :
    ```html
    <a href="https://www.example.com" target="_blank">Ouvrir dans une nouvelle fenêtre</a>
    ```

3. **`download` :** 
    
    - Cet attribut indique au navigateur de télécharger la ressource liée au lieu de la naviguer. Il est souvent utilisé avec des liens pointant vers des fichiers téléchargeables.

   - Exemple :
    ```html
    <a href="document.pdf" download>Télécharger le document</a>
   ```

4. **`rel` (Relationship) :** 
    

    - L'attribut `rel` (Relationship) de la balise `<a>` en HTML est utilisé pour définir la relation entre la page actuelle et la ressource liée. 
    
    - Cet attribut est souvent utilisé pour indiquer le type de lien ou pour fournir des informations supplémentaires sur la nature de la relation entre les deux documents.

    
    - les valeurs courantes de l'attribut `rel` :

        - **`nofollow` :** 
            
            - Indique aux **moteurs de recherche** de ne pas suivre le lien. Cela signifie que le moteur de recherche ne prendra pas en compte ce lien pour le classement des pages.

            - **Exemple :**
                ```html
                <a href="https://www.example.com" rel="nofollow">Example.com</a>
                ```

        - **`noopener` :** 
            
            - Indique que le navigateur ne doit pas ouvrir une nouvelle fenêtre ou un nouvel onglet avec accès au contexte de l'opener (la page d'origine). Cela peut aider à prévenir certaines attaques de sécurité.

            
            - **Exemple :**
                
                ```html
                <a href="https://www.example.com" rel="noopener">Example.com</a>
                ```

        - **`noreferrer` :** 
            
            - Indique que le navigateur ne doit pas envoyer d'en-têtes `Referer` lorsqu'il suit le lien. Cela peut également contribuer à renforcer la confidentialité.

            
            - **Exemple :**

                ```html
                <a href="https://www.example.com" rel="noreferrer">Example.com</a>
                ```

        - **`stylesheet` :** Indique que le lien pointe vers une feuille de style externe (généralement un fichier CSS).

            - **Exemple :**
            ```html
            <a href="style.css" rel="stylesheet">Feuille de style</a>
            ```

        - **`alternate` :** 
            
            - Indique qu'il s'agit d'une version alternative de la page actuelle. C'est souvent utilisé dans les liens de syndication pour indiquer une version alternative d'un contenu, comme une version imprimable.

            - **Exemple :**
            ```html
            <a href="printable.html" rel="alternate">Version imprimable</a>
            ```




5. **`title` :** 
    
    - Cet attribut fournit un texte explicatif qui apparaît généralement lorsque la souris survole le lien. 
    
    - Il donne des informations supplémentaires sur la destination du lien.

   - Exemple :
    ```html
    <a href="https://www.example.com" title="Site Example">Visitez Example.com</a>
    ```



### d. **les valeures de `herf`:**


- L'attribut `href` (HyperReference) de la balise `<a>` en HTML accepte diverses valeurs pour spécifier la destination du lien. 


- Voici quelques-unes des valeurs couramment utilisées :

    1. **Lien vers une page Web :**
    ```html
    <a href="https://www.example.com">Visitez Example.com</a>
    ```

    2. **Lien vers une section dans la même page (ancre) :**
    ```html
    <a href="#sectionID">Aller à la Section</a>
    <!-- ... -->
    <section id="sectionID">
        <!-- Contenu de la section -->
    </section>
    ```

    3. **Lien vers une section dans une autre page :**
    ```html
    <a href="autrepage.html#sectionID">Aller à la Section sur une autre page</a>
    ```

    4. **Lien vers un document PDF :**
    ```html
    <a href="document.pdf" >Télécharger le Document PDF</a>
    ```

    5. **Lien vers une image :**
    ```html
    <a href="image.jpg">Voir l'Image</a>
    ```

    6. **Lien vers une adresse e-mail :**
    ```html
    <a href="mailto:info@example.com">Envoyer un E-mail</a>
    ```

    7. **Lien vers un numéro de téléphone :**
    ```html
    <a href="tel:+123456789">Appeler</a>
    ```

    8. **Lien vers un fichier téléchargeable (avec l'attribut `download`) :**
    ```html
    <a href="document.zip" download>Télécharger le Document ZIP</a>
    ```

    9. **Lien vers une autre ressource (non Web) :**
    ```html
    <a href="autreresource">Autre Ressource</a>
    ```

    10. **Lien vers une ancre vide (#) pour revenir en haut de la page :**
        ```html
        <a href="#">Retour en Haut</a>
        ```


## 2. **Images en HTML:**



- **Définition:**   
    - Les balises `<img>` sont utilisées pour incorporer des images dans une page HTML. 

- **Structure de base :**

    ```html
    <img src="chemin_vers_l_image" alt="Texte de remplacement">
    ```

    - `src` (Source) spécifie le chemin de l'image.
    - `alt` (Texte de remplacement) fournit un texte alternatif si l'image ne peut pas être affichée.

- **Exemple :**

    ```html
    <img src="image.jpg" alt="Une belle image">
    ```


- **Lien autour d'une image :**

    - Vous pouvez également envelopper une balise `<a>` autour d'une balise `<img>` pour créer un lien cliquable autour de l'image.

    ```html
    <a href="lien_de_la_page">
    <img src="image.jpg" alt="Description de l'image">
    </a>
    ```

- **Attributs supplémentaires :**

    - Il existe d'autres attributs que vous pouvez utiliser pour contrôler la taille, l'alignement, etc. d'une image. Par exemple :

        ```html
        <img src="image.jpg" alt="Description de l'image" width="300" height="200" style="border: 1px solid #000;">
        ```



