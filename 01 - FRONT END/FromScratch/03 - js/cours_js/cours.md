# Cours d'initiation à JavaScript

## Qu'est-ce que JavaScript ?

**JavaScript (JS)** est un **langage de programmation de scripts** principalement utilisé pour rendre les pages web interactives. Contrairement à HTML et CSS qui définissent respectivement la structure et le style d'une page, JS permet d'ajouter des comportements dynamiques. Il est exécuté directement par le navigateur web du visiteur.

---

## Popularité de JS

JS est l'un des langages de programmation les plus populaires au monde. Sa popularité est due à plusieurs raisons, notamment sa capacité à être utilisé à la fois sur le **front-end** (côté client, dans le navigateur) et le **back-end** (côté serveur, grâce à des environnements comme Node.js). C'est un outil essentiel pour tout développeur web.

---

## Où s'écrit le JS ?

Le code JavaScript peut être intégré dans une page HTML de trois manières principales :

* **Dans la balise `<script>`** : Le code est inséré directement dans la page HTML, généralement dans la section `<head>` ou `<body>`.
* **Dans un fichier externe** : C'est la méthode la plus courante. Le code est placé dans un fichier avec l'extension `.js` et est lié à la page HTML via la balise `<script>` avec l'attribut `src`.
* **Dans les événements HTML** : Le code est directement écrit dans les attributs des balises HTML, comme `onclick` ou `onmouseover`.

---

## La syntaxe

La syntaxe de JS est simple et ressemble à celle d'autres langages comme le C, C++ ou Java. Une instruction se termine par un **point-virgule (`;`)**, bien qu'il ne soit pas toujours obligatoire, il est recommandé pour éviter les erreurs. Le code est sensible à la casse (par exemple, `MaVariable` n'est pas la même chose que `mavariable`).

---

## Les variables

Une **variable** est un conteneur qui stocke une valeur. En JavaScript, une variable peut être déclarée avec les mots-clés :

* **`var`** : L'ancienne manière de déclarer une variable. Sa portée est plus large (globale ou fonction).
* **`let`** : Pour les variables qui peuvent être réassignées. Sa portée est limitée au bloc de code où elle est déclarée.
* **`const`** : Pour les variables dont la valeur ne changera pas. Comme `let`, sa portée est limitée au bloc.

---

## La concaténation

La **concaténation** est l'action de combiner deux chaînes de caractères (du texte) en une seule. Elle est réalisée en utilisant l'opérateur **plus (`+`)**.

Exemple :  
``` js ```
let nomComplet = "Jean" + " " + "Dupont";

## Les types de données

En JS, une variable peut stocker différents types de données. Les plus courants sont :

- **String** : Une chaîne de caractères (texte).
- **Number** : Un nombre (entier ou décimal).
- **Boolean** : Une valeur de vérité (`true` ou `false`).
- **Array** : Un tableau qui contient une liste de valeurs.
- **Object** : Une collection de paires clé-valeur.
- **Null** : Indique l’absence intentionnelle de toute valeur d’objet ou de primitive.
- **Undefined** : Indique qu’une variable a été déclarée mais n’a pas encore reçu de valeur.

---

## Les opérateurs

Les opérateurs sont des symboles qui effectuent des opérations sur des valeurs.

- **Opérateurs arithmétiques** : `+`, `-`, `*`, `/` pour les calculs.
- **Opérateurs de comparaison** : `==` (égalité), `===` (égalité stricte), `!=` (inégalité), `<` (inférieur), `>` (supérieur), etc.
- **Opérateurs logiques** : `&&` (ET), `||` (OU), `!` (NON).
- **Opérateurs d’affectation** : Permettent d’assigner une valeur à une variable. L’opérateur principal est le signe égal (`=`). On trouve aussi `+=`, `-=`, etc., qui sont des raccourcis.

---

## Les structures de contrôle

Les structures de contrôle permettent de diriger le flux d’exécution du code en fonction de certaines conditions.

- **if...else** : Exécute un bloc de code si une condition est vraie, et un autre si elle est fausse.
- **switch** : Permet de choisir parmi plusieurs blocs de code à exécuter.
- **Boucles** :
  - **for** : Répète un bloc de code un nombre de fois défini.
  - **while** : Répète un bloc de code tant qu’une condition reste vraie.

---

## Les fonctions

Une **fonction** est un bloc de code réutilisable qui exécute une tâche spécifique. Elle peut accepter des **arguments** (données d’entrée) et renvoyer une **valeur** en résultat. Les fonctions sont essentielles pour organiser et structurer le code.

---

## La portée des variables

La **portée (scope)** d’une variable définit l’accessibilité de cette variable dans le code.

- **Portée globale** : La variable est accessible de partout dans le programme.
- **Portée locale** : La variable est accessible uniquement à l’intérieur de la fonction ou du bloc où elle a été déclarée. Les variables déclarées avec `let` et `const` ont une portée de bloc.