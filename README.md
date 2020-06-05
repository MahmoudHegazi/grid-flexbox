# first thing:
Grid = layout first while Flexbox = text-first or content first

# grid-flexbox
grid and flex box example 

# layout1:
<img src="mylayout1.PNG">

# layout2:
<img src="layout2.PNG">

# layout3:
<img src="layout3.PNG">


# top notes:

*  repeat(4, fr) (Create 4 same size columns or row you can use pixels "4 = numbers of elemnts you had"
*  grid-auto-rows: minmax(100px, auto)(Faceback timline or Unkown rows) it replace reapte don't forget:
minmax (100px, auto) = the min size = 100px the max size = auto (the size of content even if 9999px)

* use with grid-template-rows: 1fr 1fr (better)


# final
if we have 12 cells so if we used grid-row: 1 / 3; it will have 4 cells from our 12
if we use it like this 2/4  it will have 6 

```html

.layout {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  // same as:
  // grid-template-columns: repeat(3, 1fr);
  grid-gap: 8px;
}
.child {
  min-height: 100px;
  background: orange;
  line-height: 100px;
  text-align: center;
}

```


second:

```html
.layout {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-gap: 8px;
}
.child {
  background: orange;
  text-align: center;
  padding: 25px;
  
  display: flex;
  justify-content: space-between;
}
.last-row {
  grid-column: 1 / 3;
}

```


## Important example (Helpful)

It don't care xd top header but it must be in grid-area

```html
  grid-template: [header-left] "xd xd" 30px [header-right]
                 [main-left]   "nav  main" 1fr  [main-right]
                 [footer-left] "foot  foot" 30px [footer-right]
                 / 120px 1fr;
 /* try change foot foot to nav foot */
header {
  background-color: lime;
  grid-area: xd;
}

nav {
  background-color: lightblue;
  grid-area: nav;
}

main {
  background-color: yellow;
  grid-area: main;
}

footer {
  background-color: red;
  grid-area: foot;  
}


```

```html

grid-template-rows: repeat(12, 100px);
or
grid-template-rows: repeat(auto, 100px);

```

# Grid Gift:

```css
    grid-template: 

      "hd hd hd hd" 300px
      "sd main main main" 300px
      "ft ft ft ft" 100px 
      /  100px auto 200px;
  }
```


```css
.item-a {
  grid-column-start: 2;
  grid-column-end: five;
  grid-row-start: row1-start;
  grid-row-end: 3;
}
```

# Help ful links:
https://css-tricks.com/snippets/css/complete-guide-grid/
