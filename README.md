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

![Responsive lg](/src/assets/responsive.png)


![Responsive lg](/src/assets/responsive-xs.png)


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

![Fluid lg](/src/assets/fluid.png)


```css
.col-xs-6 {
  flex-basis: 50%;
}
```