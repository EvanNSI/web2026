### Des notions de HTML

1. HTML
HyperText Markup Language (language de balise hypertexte)

=> un fichier `.html` c'est d'abord du texte
=> il est écrit par un `développeur` (écrit avec VSCode par exemple) 
=> il est vu par un utilisateur (avec Firefox par exemple)


Une balise html s'écrit : `<maBalise></maBalise>`

**Ex:** `<h1></h1>`

Le texte s'écrit **entre les balises**.

**Ex:** `<h1>Mon texte</h1>`

Il existe aussi des balises orphelines : `<!DOCTYPE html>, <br>, <img>, ...`

Référence : Mozilla [https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements)

Une balise ouvrante peut contenir un attribut notamment `class=""` : 

`<h1 class="maClasse"></h1>`

Quelques balises importantes:
- `<h1></h1>`  : pour faire des titres
- `<p></p>`  : pour faire des paragraphes
- `<a href=""></a>`  : pour faire des liens
- `<ul></ul>`  : pour faire des listes sans ordre
- `<ol></ol>`  : pour faire des listes avec ordre
- `<li></li>`  : pour faire des items de liste
- `<img src="">`  : pour ajouter une image 

Pour trouver le chemin vers un fichier, on peut regarder:
- dans le dossier courant avec `./`
- dans un dossier extérieur avec `../`


2. CSS 

Cascading Style Sheet : Page de style en cascade

On peut écrire du CSS:
- directement dans le fichier HTML entre les balises `<style></style>`
- dans un fichier `.css` en indiquant le chemin dans le fichier HTML grâce à la balise '<link>'


Pour écrire du CSS, il faut un sélecteur (nom d'une balise ou d'une class), des accolades, des propriétés, des valeurs.

```css
selecteur{
    propriete1 : valeur1;
    propriete2 : valeur2;
    ....
}
```

Il existe plus de 500 propriétés et encore davantage de valeur possibles. 
Cependant, les valeurs sont souvent: 
- une couleur : un nom, un code (rgb(0-255,0-255,0-255,))
- une taille : il existe de nombreuses unités, pixels (px), pourcentage (%), ...

Remarque: on trouve toutes les propriétés sur le site des développeurs de Mozilla.

Les propriétés CSS s'appliquent en cascade : des éléments les plus globaux (`body`, `div`) vers les éléments les plus internes (pour finir par les classes).

Remarque : Prinicpe du modèle en boîte
Les éléments d'une page sont contenus dans une boîte entourée d'une bordure (invisible par défaut).
L'espace entre : 
- Le contenu et la bordure s'appelle `padding`.
- La bordure et les éléments autour s'appelle `margin`.

La bordure `border` peu même avoir un style.
[https://www.w3schools.com/css/css_boxmodel.asp](https://www.w3schools.com/css/css_boxmodel.asp)


Remarque : Les conteneurs universels `<div></div>` et `<span></span>`.


Il existe de nombreuses propriétés relatives au texte :
- `text-align`
- `font`

3. Javascript (JS)

C'est le language de programmation qui permet de gérer les éléments interactifs d'une page HTML.

Historiquement, les éléments d'intéractions étaient placés dans un formulaire `<form></form>` pour renvoyer des informations au serveur.

Dans le formulaire on place les éléments `<input type="">` :
- type="text"
- type="checkbox"
- type="button"