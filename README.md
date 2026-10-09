# Le rail monadique

Une page interactive qui explique les monades par l'animation, en trois temps :

1. **`fmap`** applique une fonction à l'intérieur de la boîte. Si la fonction renvoie elle-même une boîte, les couches s'imbriquent.
2. **`join`** fusionne deux couches du même contexte en une seule. Chaque monade le définit à sa façon.
3. **`>>=`** enchaîne les deux : `fmap` puis `join` à chaque étape, représenté comme un rail avec ses aiguillages.

Huit monades : `Maybe`, `Either`, `List`, `Reader`, `Writer`, `State`, `IO` et `Parser`. Le code est affiché au choix en Haskell (avec les notations `>>=` et `do`) ou en Elm (`andThen` et `|>`).

## Utilisation

Version en ligne : https://ccomb.github.io/rail-monadique/

Tout tient dans `index.html` : pas de dépendance ni d'étape de build, seulement des polices Google Fonts. Ouvrez le fichier dans un navigateur, ou servez le dossier avec n'importe quel serveur statique.
