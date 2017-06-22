# Workshop: Dominando CSS Layouts na prática com Grid Layout

### [Slides Apresentados no Workshop](https://speakerdeck.com/simoneas02/workshop-dominando-css-layouts-na-pratica-com-grid-layout) 
### [YouTube Layout - Demo](simoneas02.github.io/youtube-css-grid)

<hr>

- [História do CSS Layout](https://www.youtube.com/watch?v=94aYg5D8N0s&t=58s)
- [O que é CSS Grid Layout](https://www.w3.org/TR/css-grid-1/)
- [CSS Grid Layout x Flexbox]()
- [Terminologia](https://codepen.io/simoneas02/post/grid-layout)
    - Grid Lines
    - Grid Track
    - Grid Cell
    - Grid Area
<hr>

## [Collection Workshop](bit.ly/css-grid-layouts)

### [01 - Definindo um Grid](bit.ly/01-definindo-grid)

```CSS
    display: grid
    display: inline-grid
```

### [02 - Line Base Placement](bit.ly/02-placement)

```CSS
    grid-template-columns: 50px 100px 200px;
    grid-template-rows: 100px 150px;
```

### [03 - Line Base Position](bit.ly/03-position)

```CSS
    .e {
        grid-column-start: 1;
        grid-column-end: 3;
        grid-row-start: 1;
        grid-row-end: 2;
    }
```

### [04 - Line Base Position - Shorthands](bit.ly/04-position-shorthands)

```CSS
    .e {
        grid-column: 1 / 4;
        grid-row: 1 / 2;
    }

    .d {
        grid-area: 1 / 1 / 2 / 3;
    }
```

### [05 - Grid Gap](bit.ly/05-grid-gap)

```CSS
    grid-column-gap: 10px;
    grid-row-gap: 20px;

    grid-gap: 10px 20px;

    grid-gap: 20px;
```

- [06 - Area Naming](bit.ly/06-area-naming)

```CSS
    grid-template-areas:
        "header header header"
        "nav content aside"
        "footer footer footer";

    grid-area: header;
    grid-area: nav;
    grid-area: content;
    grid-area: aside;
    grid-area: footer;

/* Responsive Web Design */

@media(max-width: 590px) {
    .grid-container {
        grid-template-columns: 25% 75%;
        grid-template-rows: 20% 10% 50% 20%;
        grid-template-areas:
        "header header"
        "nav nav"
        "content aside"
        "footer footer";
    }
}

    @media(max-width: 450px) {
    .grid-container {
        grid-template-columns: 100%;
        grid-template-rows: 20% 10% 10% 50% 10%;
        grid-template-areas:
        "header"
        "nav"
        "content" 
        "aside"
        "footer";
    }
}
```
<hr>

- [Hands On - YouTube Layout ]()
- [Suporte](https://caniuse.com/#feat=css-grid)
- [Quer saber mais](https://github.com/simoneas02/awesome-grid-layout)
