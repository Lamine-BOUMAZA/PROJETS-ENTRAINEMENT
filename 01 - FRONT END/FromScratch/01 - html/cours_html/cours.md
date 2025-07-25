# Cours HTML

## Table des matières
- [Cours HTML](#cours-html)
  - [Table des matières](#table-des-matières)
  - [Navigation](#navigation)
  - [En-tête](#en-tête)
  - [Listes](#listes)
    - [Liste ordonnée](#liste-ordonnée)
  - [Images](#images)
  - [Tableaux](#tableaux)
  - [Liens](#liens)
  - [Vidéos](#vidéos)
  - [Formulaires](#formulaires)
  - [Footer](#footer)

---

## Navigation

```html
<nav>
  <!-- UL = Unordered List -->
  <ul>
    <li>Accueil</li>
    <li>Boutique</li>
    <li><a href="#form">Formulaire</a></li>
  </ul>
</nav>
```

- `<nav>` définit la zone de navigation.
- `<ul>` crée une liste non ordonnée.
- `<li>` définit chaque élément de la liste.

---

## En-tête

```html
<header>
  <!-- La bonne pratique est qu'on doit mettre un seul h1 par page ! -->
  <h1>Ceci est le titre principal</h1>
  <p>
    Ceci est un paragraphe
    <em>Texte en italique : balise -> em</em>
    <strong>Texte en gras : balise -> strong</strong>
    Besoin d'un texte afin de placer plus tard du contenu (lorem50 donc 50 mots) Lorem ipsum dolor sit amet...
  </p>
</header>
```

- `<header>` regroupe le titre principal et un paragraphe.
- `<h1>` est le titre principal de la page (un seul par page).
- `<em>` met le texte en italique.
- `<strong>` met le texte en gras.

---

## Listes

### Liste ordonnée

```html
<section>
  <!-- OL = Ordered List -->
  <h2>Ordered List</h2>
  <ol>
    <li>Ceci est une</li>
    <li>liste dans</li>
    <li>l'ordre</li>
  </ol>
</section>
```

- `<ol>` crée une liste ordonnée (numérotée).
- `<li>` définit chaque élément.

---

## Images

```html
<section>
  <h3>Image en HTML</h3>
  <img src="./ressources/images/HTML5_logo_and_wordmark.svg.png" height="150" width="150" alt="image_section_3">
</section>
```

- `<img>` insère une image avec attributs `src`, `height`, `width` et `alt`.

---

## Tableaux

```html
<div>
  <h4>Tableaux</h4>
  <table border="5" cellpadding="10" cellspacing="5" style="text-align: center;">
    <thead>
      <tr>
        <th>Col 1</th>
        <th>Col 2</th>
        <th>Col 3</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td rowspan="2">Cell 1</td>
        <td>Cell 2</td>
        <td>Cell 3</td>
      <tr>
        <td colspan="2">Cell 4</td>
      </tr>
      </tr>
    </tbody>
  </table>
</div>
```

- `<table>` crée un tableau.
- `<thead>`, `<tbody>`, `<tr>`, `<th>`, `<td>` structurent le tableau.
- Attributs `rowspan` et `colspan` fusionnent des cellules.

---

## Liens

```html
<div>
  <h5><i>&#10148;</i> Les liens</h5>
  <a href="https://htmlcheatsheet.com" target="_blank">HTML Cheat Sheet</a>
  <!-- _blank permet d'ouvrir le lien dans un autre onglet -->
</div>
```

- `<a>` crée un lien hypertexte.
- Attribut `target="_blank"` ouvre le lien dans un nouvel onglet.

---

## Vidéos

```html
<div>
  <h6> <span>&#128249;</span> Les vidéos</h6>
  <video src="./ressources/videos/istockphoto-545625782-640_adpp_is.mp4" height="200" autoplay muted loop></video>
</div>
```

- `<video>` permet d’intégrer une vidéo avec options d’autoplay, muet et boucle.

---

## Formulaires

```html
<section id="form">
  <h2>Les Formulaires</h2>
  <form action="">
    <!-- for et id permettent de lier le label à l'input -->
    <label for="name">Nom</label>
    <input id="name" type="text" placeholder="Entrez votre nom" />

    <br/>

    <label for="age">Âge</label>
    <input id="age" type="number" placeholder="Entrez votre âge" />

    <br />

    <!-- input de type select  -->
    <label for="gender">Genre</label>
    <select name="" id="gender">
      <option value="Homme">Homme</option>
      <option selected="selected" value="Femme">Femme</option>
    </select>

    <div>
      <input type="radio" name="type" id="human" checked>
      <label for="human">Humain</label>

      <input type="radio" name="type" id="dog">
      <label for="dog">Chien</label>

      <input type="radio" name="type" id="cat">
      <label for="cat">Chat</label>
    </div>
    <textarea placeholder="Votre message..."></textarea>

    <br>

    <!-- input de type checkbox -->
    <input type="checkbox" name="" id="cgv">
    <label for="cgv">Accepter les CGV</label>

    <br>

    <input type="submit" value="Ceci est le bouton pour valider le form">
  </form>
  <button>Ceci est le bouton pour valider le form</button>
</section>
```

- `<form>` regroupe les champs du formulaire.
- `<label>` associé à un `<input>` via l’attribut `for`.
- `<input>` pour les champs texte, nombre, radio, checkbox, bouton.
- `<select>` pour les listes déroulantes.
- `<textarea>` pour les zones de texte.

---

## Footer

```html
<footer>
  <a href="mailto:azerty@gmail.com">Contactez-moi</a>
  <a href="./notice.txt" download="notice">À télécharger</a>
</footer>
```

- `<footer>` contient les informations de bas de page.
- Lien mailto pour envoyer un mail, lien de téléchargement.

---

> **Astuce** :  
> Pour chaque balise, pense à bien utiliser les attributs adaptés (`alt` pour les images, `for` pour les labels, etc.) et à structurer ton HTML pour la lisibilité