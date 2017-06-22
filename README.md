# Workshop: Dominando CSS Layouts na prática com Grid Layout

### [Slides Apresentados no Workshop](https://speakerdeck.com/simoneas02/workshop-dominando-css-layouts-na-pratica-com-grid-layout) 
### [Acesse o pojeto YouTube Layout online](https://simoneas02.github.io/youtube-css-grid/)

![YouTube Layout - Demo](./final/assets/img/demo.gif)

<hr>

- [História do CSS Layout](https://www.youtube.com/watch?v=94aYg5D8N0s&t=58s)
- [O que é CSS Grid Layout](https://www.w3.org/TR/css-grid-1/)
- [CSS Grid Layout x Flexbox](https://rachelandrew.co.uk/archives/2016/03/30/should-i-use-grid-or-flexbox/)
- [Terminologia](https://codepen.io/simoneas02/post/grid-layout)
    - Grid Lines
    - Grid Track
    - Grid Cell
    - Grid Area
<hr>

## [Collection Workshop](https://codepen.io/collection/AdOVGW/)

### [01 - Definindo um Grid](https://codepen.io/simoneas02/pen/gRRLRb)

```CSS
    display: grid
    display: inline-grid
```

### [02 - Line Base Placement](https://codepen.io/simoneas02/pen/qjjqyw)

```CSS
    grid-template-columns: 50px 100px 200px;
    grid-template-rows: 100px 150px;
```

### [03 - Line Base Position](https://codepen.io/simoneas02/pen/LLLbXK)

```CSS
    .e {
        grid-column-start: 1;
        grid-column-end: 3;
        grid-row-start: 1;
        grid-row-end: 2;
    }
```

### [04 - Line Base Position - Shorthands](https://codepen.io/simoneas02/pen/BZZQeW)

```CSS
    .e {
        grid-column: 1 / 4;
        grid-row: 1 / 2;
    }

    .d {
        grid-area: 1 / 1 / 2 / 3;
    }
```

### [05 - Grid Gap](https://codepen.io/simoneas02/pen/GEEror)

```CSS
    grid-column-gap: 10px;
    grid-row-gap: 20px;

    grid-gap: 10px 20px;

    grid-gap: 20px;
```

### [06 - Area Naming](https://codepen.io/simoneas02/pen/LLLxLp)

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

- [Hands On - YouTube Layout ](https://github.com/simoneas02/youtube-css-grid/tree/master/training)
- [Suporte](https://caniuse.com/#feat=css-grid)
- [Quer saber mais](https://github.com/simoneas02/awesome-grid-layout)
