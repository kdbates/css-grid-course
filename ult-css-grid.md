# Ultimate CSS Grid Course: From Beginner to Advanced
[Udemy Course from Peter Sommerhof](https://www.udemy.com/css-grid/learn/v4/content)

## Source-Order Independence: order
pick up at [Section 3 #14](https://www.udemy.com/css-grid/learn/v4/t/lecture/7943450?start=0)

## Defining Gutters (gaps): grid-row-gap & grid-column-gap
```css
.grid {
  display: grid;
  grid-template: 100px 100px
    / 200px auto 150px;
  grid-row-gap: 10px;
  grid-column-gap: 10px
}
```
### Shorthand version
```css
.grid {
  display: grid;
  grid-template: 100px 100px
    / 200px auto 150px;
  /* grid-row-gap: 10px; */
  /* grid-column-gap: 10px */
  grid-gap: 10px;
}
```

## Naming Grid Lines
Give **EXPLICIT** names to your grid lines.  
Use square brackets to designate names in the code, i.e. 
```css
.grid {
  display: grid;
  grid-template: [row1-start] 100px [row1-end row2-start] 100px [row2-end]
    /200px auto 150px;
}
```


## Spanning a Fixed Number of Rows or Columns
```css
.grid div:nth-child(1) {
  grid-row: auto / span 2;
}
```

## Arranging grid items with start and end
### Long Hand Version
```css
.grid div:nth-child(2) {
  grid-row-start: 2;
  grid-row-end: 3;
  grid-column-start: 1;
  grid-column-end: 2;
}
```
### Short Hand Version
```css
.grid div:nth-child(5) {
  grid-row: 1 / 2;
  grid-column: 1 / 2;
}
```

## grid-template-rows & grid-template-columns
```grid-template``` is shorthand to define first rows and then columns in your design.
```css
.grid {
  display: grid;
  grid-template: 100px 100px 
  / 200px auto 150px;
}
```

## display:grid
```css
.grid {
  display: grid;
}
```