# Cours Complet sur le HTML

## Table des matières
- [Cours Complet sur le HTML](#cours-complet-sur-le-html)
  - [Table des matières](#table-des-matières)
  - [1. Introduction et structure de base](#1-introduction-et-structure-de-base)
  - [2. Les balises essentielles](#2-les-balises-essentielles)
  - [3. Commentaires](#3-commentaires)
  - [4. Les balises sémantiques](#4-les-balises-sémantiques)
  - [5. Les listes](#5-les-listes)
    - [Liste non ordonnée](#liste-non-ordonnée)
    - [Liste ordonnée](#liste-ordonnée)
  - [6. Les images et multimédias](#6-les-images-et-multimédias)
    - [Image](#image)
    - [Vidéo](#vidéo)
    - [Audio](#audio)
  - [7. Les liens et ancres](#7-les-liens-et-ancres)
    - [Lien externe](#lien-externe)
    - [Lien interne (ancre)](#lien-interne-ancre)
    - [Lien mailto et téléchargement](#lien-mailto-et-téléchargement)
  - [8. Les tableaux](#8-les-tableaux)
  - [9. Les formulaires](#9-les-formulaires)
  - [10. Accessibilité](#10-accessibilité)
  - [11. Bonnes pratiques](#11-bonnes-pratiques)
  - [12. Ressources utiles](#12-ressources-utiles)

---

## 1. Introduction et structure de base

Le HTML (HyperText Markup Language) est le langage de base pour structurer le contenu d’une page web.

```html
<!DOCTYPE html>
<html lang="fr">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Titre de la page</title>
    <link rel="shortcut icon" href="favicon.ico" />
  </head>
  <body>
    <!-- Contenu de la page -->
  </body>
</html>
```

- `<!DOCTYPE html>` : Indique au navigateur qu’il s’agit d’un document HTML5.
- `<html lang="fr">` : Racine du document, avec la langue.
- `<head>` : Métadonnées, titre, liens externes.
- `<body>` : Contenu visible de la page.

---

## 2. Les balises essentielles

- `<h1>` à `<h6>` : Titres (un seul `<h1>` par page).
- `<p>` : Paragraphe.
- `<br>` : Saut de ligne.
- `<hr>` : Ligne horizontale.
- `<strong>` : Texte important (gras).
- `<em>` : Texte accentué (italique).
- `<span>` : Pour styliser une portion de texte.
- `<div>` : Division générique de contenu.

---

## 3. Commentaires

Les commentaires servent à documenter le code et ne sont pas affichés dans le navigateur.

```html
<!-- Ceci est un commentaire -->
```

---

## 4. Les balises sémantiques

Elles donnent du sens au contenu et améliorent l’accessibilité et le référencement.

- `<header>` : En-tête de page ou de section.
- `<nav>` : Zone de navigation.
- `<main>` : Contenu principal.
- `<section>` : Section thématique.
- `<article>` : Contenu autonome.
- `<aside>` : Contenu secondaire (ex : barre latérale).
- `<footer>` : Pied de page.

---

## 5. Les listes

### Liste non ordonnée

```html
<ul>
  <li>Élément 1</li>
  <li>Élément 2</li>
</ul>
```

### Liste ordonnée

```html
<ol>
  <li>Premier</li>
  <li>Second</li>
</ol>
```

---

## 6. Les images et multimédias

### Image

```html
<img src="chemin/vers/image.jpg" alt="Description de l'image" width="200" height="100">
```
- L’attribut `alt` est essentiel pour l’accessibilité.

### Vidéo

```html
<video src="video.mp4" controls autoplay muted loop></video>
```

### Audio

```html
<audio src="audio.mp3" controls></audio>
```

---

## 7. Les liens et ancres

### Lien externe

```html
<a href="https://www.example.com" target="_blank">Visiter le site</a>
```

### Lien interne (ancre)

```html
<a href="#section2">Aller à la section 2</a>
...
<h2 id="section2">Section 2</h2>
```

### Lien mailto et téléchargement

```html
<a href="mailto:exemple@mail.com">Envoyer un mail</a>
<a href="fichier.pdf" download>Télécharger le PDF</a>
```

---

## 8. Les tableaux

```html
<table>
  <thead>
    <tr>
      <th>Colonne 1</th>
      <th>Colonne 2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Ligne 1, Cellule 1</td>
      <td>Ligne 1, Cellule 2</td>
    </tr>
    <tr>
      <td colspan="2">Cellule fusionnée</td>
    </tr>
  </tbody>
</table>
```

---

## 9. Les formulaires

```html
<form action="/traitement" method="post">
  <label for="nom">Nom :</label>
  <input type="text" id="nom" name="nom" placeholder="Votre nom" required>

  <label for="age">Âge :</label>
  <input type="number" id="age" name="age">

  <label for="genre">Genre :</label>
  <select id="genre" name="genre">
    <option value="homme">Homme</option>
    <option value="femme">Femme</option>
  </select>

  <input type="checkbox" id="cgv" name="cgv" required>
  <label for="cgv">Accepter les CGV</label>

  <input type="submit" value="Envoyer">
</form>
```

- Utiliser `label` lié à l’`input` pour l’accessibilité.
- Attributs utiles : `placeholder`, `required`, `checked`, `selected`.

---

## 10. Accessibilité

- Toujours renseigner l’attribut `alt` pour les images.
- Utiliser les balises sémantiques pour structurer la page.
- Associer les `<label>` aux `<input>` avec l’attribut `for`.
- Privilégier une structure logique des titres (`h1`, `h2`, etc.).
- Tester la navigation au clavier (tabulation).

---

## 11. Bonnes pratiques

- Indenter correctement le code.
- Utiliser un seul `<h1>` par page.
- Privilégier les balises sémantiques.
- Commenter le code pour le rendre compréhensible.
- Garder le code lisible et organisé.
- Toujours vérifier la compatibilité des balises et attributs.

---

## 12. Ressources utiles

- [MDN Web Docs (Mozilla)](https://developer.mozilla.org/fr/docs/Web/HTML)
- [W3Schools](https://www.w3schools.com/html/)
- [HTML CheatSheet](https://htmlcheatsheet.com/)
- [Validator W3C](https://validator.w3.org/)

---

> **Astuce** : Pour aller plus loin, apprends à intégrer CSS et JavaScript à tes pages