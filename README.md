#  CSS-Grid

### This is just a place for me to mess around with CSS-grid.

And so far... I'm loving it!

Snippets:
```css
body {
  display: grid;
  grid:
    "nav nav nav" auto
		"header header header" auto
		"aside main ." 766px
		"aside footer footer" 50px
    /15% auto 15%;
}

header {
	grid-area: header;
}
etc...
```

You put grids within grids... use clasname to target.

```css
main {
	grid-area: main;
	background: #f0f0f0	;
	display: grid;
	grid:
		"one two three" auto
		/ 1fr 2fr 1fr;
	grid-gap: 2em;
}
.one {
	background: blue;
}
```

`grid-gap: <grid-row-gap> <grid-column-gap>};`
if the are the same, just put one value
