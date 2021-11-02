<style>
    @import url('https://fonts.googleapis.com/css2?family=Roboto+Slab&family=Roboto:wght@300;500&display=swap');

    :root {
        --ombre: #000;
        --gris-sombre: #151525;
        --gris-bloc: #191928;

         --gris-tableau: #252533;
        --gris-moyen: #999;
        --gris-clair: #ccc;

        --html-primaire: #ADFC92;
        --html-secondaire: #7cca52;
        --html-bleu: #17BEBB;
        --css-primaire: #FF9505;
        --css-secondaire: #bb5500;

        --bleu-profond: #000815;
        --bleu-profond-hover: #00122d;
    }

    *, *::before, *::after {
        box-sizing:border-box;
    }

    html {
        font-size:50%;
    }




    body {
        display:flex;
        flex-wrap: wrap;
        justify-content: center;
        align-items: flex-start;
        background: var(--gris-sombre);
        color: var(--gris-clair);
        font-family: 'Roboto', sans-serif;
        column-gap: 4rem;
    }

    table, tr, td, th {
        border-collapse: collapse;
        border: 1px solid var(--gris-tableau);
    }

    th {
        background: var(--gris-tableau);
        color: var(--gris-moyen);
        text-align:left;
    }

    th,td {
        padding: 1rem;
    }

    code {
        margin: .2rem .8rem .2rem 0;
        padding: .5rem 1rem;
        background: var(--html-primaire);
        color: var(--gris-sombre);
        border-radius: .5rem;
        box-shadow: 0 3px var(--html-secondaire), .3rem .8rem 2rem var(--ombre);
        white-space: nowrap;
    }

   h1 {
        flex: 1 0 100%;
        color: var(--gris-clair);
        text-align:center;
        letter-spacing: .3rem;
        font-size: 4.6rem;
        font-family: 'Roboto Slab', serif;
    }

    h2 {
        background: var(--html-primaire);
        color: var(--gris-sombre);
        text-align:center;
    }

    h1, h2 {
        display: inline-block;
        padding: 0.8rem 1.8rem;
        font-weight: 500;
    }

    h3 {
        margin-top: 3.5rem;
        color:var(--css-primaire);
        font-weight: 300;
    }


    strong {
        color: var(--html-bleu);     
    }

    em {
        color: var(--html-bleu); 
    }

    ul, li {
        margin:0;
        padding:0;
    }

    li {
        list-style: disc inside;
        line-height: 2.5;
    }

    blockquote {
        position: relative;
        display: inline-block;
        padding:0;
        margin: 3rem 0;
        border: 0 none;
        border-radius: .3rem;
        background: var(--bleu-profond);
        transition:background .5s ease-out;
        word-break: break-all;        
    }
    blockquote:hover {
        background: var(--bleu-profond-hover);
        transition:background .5s ease-out;
    }

    blockquote a {
        padding-left:1.8rem;
        color: var(--html-bleu);
    }

    blockquote p {
        margin: 0;
        display: flex;
        align-items: center;
    }

    blockquote p::before {
        box-sizing: content-box;
        content:url('data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA0Ni43NTMgMTM5LjciPgogIDxwYXRoIGZpbGw9IiMxN0JFQkIiIGQ9Ik0tNDA3LjY5IDQzNy4wOWMtMTEuNTE2LjA3NC0yMi44NTcgOS42ODktMjIuODU3IDI2LjUyMXY3OC43MzZjMCA2LjYyNCAyLjIxIDExLjkwMyA1LjcyIDE1LjQwMiAzLjUxIDMuNSA4LjIgNS4xNjcgMTIuODI1IDUuMDc4IDkuMjQ4LS4xNzggMTguNDMyLTcuNzYgMTguNDMyLTIwLjQ4di02Ny42MTNjMC04LjU3NC02Ljg2My0xNC4wNDgtMTMuNjgyLTE0LjQxMi0zLjQxLS4xODItNi45NDkuODQtOS42NDMgMy4zMTQtMi42OTQgMi40NzQtNC4zNiA2LjM0MS00LjM2IDExLjA5OHY0NC40YTMgMyAwIDEgMCA2IDB2LTQ0LjRjMC0zLjQzMiAxLjA0NS01LjQxOCAyLjQxNy02LjY3N3MzLjI1NC0xLjg1IDUuMjY1LTEuNzQyYzQuMDIzLjIxNCA4LjAwMiAyLjkyOCA4LjAwMiA4LjQydjY3LjYxMmMwIDkuOTkzLTYuMzA2IDE0LjM2MS0xMi41NDcgMTQuNDgtMy4xMi4wNi02LjE3NC0xLjAzNy04LjQ3Mi0zLjMyOC0yLjI5OC0yLjI5LTMuOTU3LTUuODI0LTMuOTU3LTExLjE1MnYtNzguNzM2YzAtMTQuMjc3IDguNTM1LTIwLjQ2OCAxNi44OTYtMjAuNTIgOC4zNi0uMDU0IDE2Ljg1NyA1Ljk2OSAxNi44NTcgMjAuNTJ2NTIuOTQzYTMgMyAwIDEgMCA2IDB2LTUyLjk0M2MwLTE3LjA2Ny0xMS4zOC0yNi41OTUtMjIuODk2LTI2LjUyeiIgY29sb3I9IiMwMDAiIHN0eWxlPSJ0ZXh0LWRlY29yYXRpb24tY29sb3I6IzAwMDtpc29sYXRpb246YXV0bzttaXgtYmxlbmQtbW9kZTpub3JtYWw7YmxvY2stcHJvZ3Jlc3Npb246dGI7dGV4dC1kZWNvcmF0aW9uLWxpbmU6bm9uZTt3aGl0ZS1zcGFjZTpub3JtYWw7dGV4dC1pbmRlbnQ6MDt0ZXh0LXRyYW5zZm9ybTpub25lO3RleHQtZGVjb3JhdGlvbi1zdHlsZTpzb2xpZCIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoNDMxLjA1IC00MjMuNjMpIi8+Cjwvc3ZnPgo=');
        width: 1.2rem;
        display: inline-block;
        vertical-align: middle;
        padding: 0.7rem 1.8rem;
        background: var(--bleu-profond-hover);
    }

    .infos {
        display:flex;
        flex-flow:wrap;
        max-width:60rem;
        padding: 0 2rem 2rem;
        margin-top: 4rem;
        margin-bottom: 2rem;
        background: var(--gris-bloc);
        color: var(--gris-moyen);
        font-size: 1.5rem;
        font-weight: 500;
        border-radius: .8rem;
        box-shadow: .6rem .8rem 4.8rem var(--ombre);
        
    }

    .infos :not(h2) {
        flex-basis: 100%;
    }

    .infos>h2 {
        margin: 0;
        align-self: flex-start;
        background: --couleur-html-primaire;
        transform: translateY(-2.3rem);
    }

    .infos>h2::after {
        position: absolute;
        content:'';
        height : 0;
        width : 0;
        right: -1.8rem;
        top: -.1rem;
        border-bottom: 2.3rem solid  var(--html-secondaire);
        border-right: 1.8rem solid transparent;
    }

    .css h2 {
        background: var(--css-primaire);
    }

    .css code {
        background: var(--css-primaire);
        box-shadow: 0 .3rem var(--css-secondaire), .3rem .8rem 2rem var(--ombre);
    }

    .css h2::after {
        border-bottom-color: var(--css-secondaire);
    }

    .css strong {
        color: var(--css-primaire);     
    }

    .css td code {
        all: unset;
        padding: .8rem .5rem;
    }

    @media screen and (min-width:360px) {
        html {
            font-size:62.5%;
        }

    }
</style>

# Informations sur DM1

<div class="infos html">

## HTML

- Les éléments : `Email` `Password` `Remember me` `Forgot password?` `Login`
  sont contenus dans la même balise, `<form>`

> https://htmlreference.io/element/form/

- Utilisez la balise `<input>` pour les champs de formulaire `Email` `Password` `Remember Me` avec les attributs **type** correspondants

> https://htmlreference.io/element/input/

- Utilisez la balise `<button>` pour le bouton `Login` avec l'attribut **type** correspondant

> https://htmlreference.io/element/button/

</div>

<div class="infos css">

## CSS

- Les arrondis font tous **5px**
- La maquette a été conçu pour des écrans de **375px**

### Couleurs

| A appliquer sur   | Référence couleur                                                                   |
| ----------------- | ----------------------------------------------------------------------------------- |
| Titre             | <span style="color:#fff;background:#000000;display:inline-block;">`#000000`</span>  |
| Texte Courant     | <span style="color:#000;background:#8B959A;display:inline-block;">`#8B959A` </span> |
| Bouton Login      | <span style="color:#000;background:#3C82FF;display:inline-block;">`#3C82FF` </span> |
| Twitter           | <span style="color:#000;background:#76A9EA;display:inline-block;">`#76A9EA` </span> |
| Facebook          | <span style="color:#000;background:#475993;display:inline-block;">`#475993` </span> |
| Couleur dégradé 1 | <span style="color:#000;background:#6590DE;display:inline-block;">`#6590DE` </span> |
| Couleur dégradé 2 | <span style="color:#000;background:#A7CEFF;display:inline-block;">`#A7CEFF` </span> |

### Typos

- Utiliser une Police de caractère sur Google Font : `Roboto`

| A appliquer sur  | Taille |
| ---------------- | ------ |
| Titre            | 26px   |
| Texte courant    | 14px   |
| Champs et Bouton | 17px   |

### OPTIONNEL - DÉFI POUR LES PLUS TÉMÉRAIRES !

- En se basant sur le fichier `tablette-desktop.png`, affichez une version responsive à partir de **575px**

> https://developer.mozilla.org/fr/docs/Web/CSS/@media

- Cette version aura un fond en dégradé linéaire ( _cf tableau couleur_ )
- La taille du formulaire sera limitée à **575px**
- Le formulaire devra être **centré horizontalement** et **verticalement** dans la page
</div>
