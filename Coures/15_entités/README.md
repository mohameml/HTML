
Les entités HTML sont des séquences de caractères spéciales utilisées pour représenter des caractères réservés ou des caractères spéciaux dans le code HTML. Elles sont souvent utilisées pour éviter toute confusion avec la syntaxe HTML et pour garantir que le navigateur interprète correctement le texte.

Voici quelques-unes des entités HTML couramment utilisées :

1. **Caractères spéciaux :**
   - `&lt;` : `<` (inférieur à)
   - `&gt;` : `>` (supérieur à)
   - `&amp;` : `&` (esperluette)
   - `&quot;` : `"` (guillemet double)
   - `&apos;` : `'` (apostrophe simple)

   Exemple :
   ```html
   <p>Ceci est un exemple d'utilisation des entités : &lt;p&gt; &amp; &lt;/p&gt;</p>
   ```

2. **Caractères diacritiques (accents) :**
   - `&eacute;` : é
   - `&egrave;` : è
   - `&ecirc;` : ê
   - `&agrave;` : à

   Exemple :
   ```html
   <p>Voil&agrave; un café avec un accent &eacute; sur le &ecirc;.</p>
   ```

3. **Symboles mathématiques et autres :**
   - `&nbsp;` : espace insécable (non-breaking space)
   - `&copy;` : © (symbole de copyright)
   - `&reg;` : ® (symbole de marque déposée)
   - `&trade;` : ™ (symbole de marque commerciale)

   Exemple :
   ```html
   <p>&copy; 2024 Mon Entreprise. Tous droits réservés.</p>
   ```

Ces entités HTML permettent d'insérer des caractères spéciaux dans votre code HTML tout en garantissant une interprétation correcte par les navigateurs. Utiliser ces entités est particulièrement important lorsqu'il s'agit de caractères réservés ou de symboles ayant une signification spéciale en HTML.