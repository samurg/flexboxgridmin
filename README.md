Flexbox Grid
===========

Grid based on the `flex` display property.


### css
* [Development](https://github.com/samurg/flexboxgridmin/master/src/flexboxgrid.css)
* [Production](https://github.com/samurg/flexboxgridmin/master/dist/flexboxgrid.min.css)

Add the `flexboxgrid.css` __development__ or `flexboxgrid.min.css` __production__ to your html page.




Simple Syntax
---------

All you need to remember is row, column, content.

```html
<div class="row">
    <div class="col-xs-12">
        <div class="box">12</div>
    </div>
</div>
```

Responsive
---------

Responsive modifiers enable specifying different column sizes, offsets, alignment and distribution at xs, sm, md & lg viewport widths.


![Responsive lg](/src/assets/img/responsive.png?raw=true "Responsive lg")

![Responsive xs](/src/assets/img/responsive-xs.png?raw=true "Responsive xs")


```html
<div class="row">
    <div class="col-xs-12
                col-sm-8
                col-md-6
                col-lg-4">
        <div class="box">Responsive</div>
    </div>
</div>
```


Fluid
---------

Percent based widths allow fluid resizing of columns and rows.

![Fluid lg](/src/assets/img/fluid.png)


```css
.col-xs-6 {
  flex-basis: 50%;
}
```


Offsets
---------

Offset a column

![Offsets lg](/src/assets/img/offsets-lg.png?raw=true "Offsets lg")


```html
<div class="row">
    <div class="col-xs-offset-3 col-xs-9">
        <div class="box">offset</div>
    </div>
</div>
```


Auto Width
---------

Add any number of auto sizing columns to a row. Let the grid figure it out.

![Auto Width lg](/src/assets/img/auto-width-lg?raw=true "Auto Width")


```html
<div class="row">
    <div class="col-xs">
        <div class="box">auto</div>
    </div>
</div>
```


Nested Grids
---------

Nest grids inside grids inside grids.

![Nested Grids lg](/src/assets/img/netsed-grid-lg?raw=true "Nested Grids")


```html
<div class="row">
    <div class="col-xs">
        <div class="box">
            <div class="row">
                <div class="col-xs">
                    <div class="box">auto</div>
                </div>
            </div>
        </div>
    </div>
</div>
```


Alignment
---------

Add classes to align elements to the start or end of a row as well as the top, bottom, or center of a column

- .start-

![Alignment Start](/src/assets/img/alignment-start?raw=true "Alignment Start")


```html
<div class="row start-xs">
    <div class="col-xs-6">
        <div class="box">
            start
        </div>
    </div>
</div>
```

- .center-

![Alignment Center](/src/assets/img/alignment-center?raw=true "Alignment Center")


```html
<div class="row center-xs">
    <div class="col-xs-6">
        <div class="box">
            center
        </div>
    </div>
</div>
```

- .end-

![Alignment End](/src/assets/img/alignment-end?raw=true "Alignment End")


```html
<div class="row end-xs">
    <div class="col-xs-6">
        <div class="box">
            end
        </div>
    </div>
</div>
```

Here is an example of using the modifiers in conjunction to acheive different alignment at different viewport sizes.

![Alignment Example](/src/assets/img/alignment-example?raw=true "Alignment Example")

Example:

```html
<div class="row center-xs end-sm start-lg">
    <div class="col-xs-6">
        <div class="box">
            All together now
        </div>
    </div>
</div>
```

- .top-

![Alignment Top](/src/assets/img/alignment-top?raw=true "Alignment Top")


```html
<div class="row top-xs">
    <div class="col-xs-6">
        <div class="box">
            top
        </div>
    </div>
</div>
```


- .middle-

![Alignment Middle](/src/assets/img/alignment-middle?raw=true "Alignment Middle")


```html
<div class="row middle-xs">
    <div class="col-xs-6">
        <div class="box">
            middle
        </div>
    </div>
</div>
```

- .bottom-

![Alignment Bottom](/src/assets/img/alignment-bottom?raw=true "Alignment Bottom")


```html
<div class="row bottom-xs">
    <div class="col-xs-6">
        <div class="box">
            bottom
        </div>
    </div>
</div>
```


Distribution
---------

Add classes to distribute the contents of a row or column.

- .around-

![Distribution around](/src/assets/img/distribution-arround?raw=true "Distribution around")


```html
<div class="row around-xs">
    <div class="col-xs-2">
        <div class="box">
            around
        </div>
    </div>
    <div class="col-xs-2">
        <div class="box">
            around
        </div>
    </div>
    <div class="col-xs-2">
        <div class="box">
            around
        </div>
    </div>
</div>
```


- .between-

![Distribution between](/src/assets/img/distribution-between?raw=true "Distribution between")


```html
<div class="row between-xs">
    <div class="col-xs-2">
        <div class="box">
            between
        </div>
    </div>
    <div class="col-xs-2">
        <div class="box">
            between
        </div>
    </div>
    <div class="col-xs-2">
        <div class="box">
            between
        </div>
    </div>
</div>
```


Reordering
---------

Add classes to reorder columns.

- .first-

![Reordering first](/src/assets/img/reordering-first?raw=true "Reordering first")


```html
<div class="row">
    <div class="col-xs-2">
        <div class="box">
            1
        </div>
    </div>
    <div class="col-xs-2">
        <div class="box">
            2
        </div>
    </div>
    <div class="col-xs-2 first-xs">
        <div class="box">
            3
        </div>
    </div>
</div>
```


- .last-

![Reordering last](/src/assets/img/reordering-last?raw=true "Reordering last")


```html
<div class="row">
    <div class="col-xs-2 last-xs">
        <div class="box">
            1
        </div>
    </div>
    <div class="col-xs-2">
        <div class="box">
            2
        </div>
    </div>
    <div class="col-xs-2">
        <div class="box">
            3
        </div>
    </div>
</div>
```


Reversing
---------

- .reverse-

![Reversing reverse](/src/assets/img/reversing-reverse?raw=true "Reversing reverse")


```html
<div class="row reverse">
    <div class="col-xs-2">
        <div class="box">
            1
        </div>
    </div>
    <div class="col-xs-2">
        <div class="box">
            2
        </div>
    </div>
    <div class="col-xs-2">
        <div class="box">
            3
        </div>
    </div>
</div>
```
