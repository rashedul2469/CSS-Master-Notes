# CSS Documentation

## Table of Contents

- [Basic CSS Structure](#basic-css-structure)
- [CSS Type](#css-type)
  - [Inline CSS](#inline-css)
  - [Internal CSS](#internal-css)
  - [External CSS](#external-css)
- [CSS Selector](#css-selector)
  - [Simple Selectors](#simple-selectors)
  - [Combinator Selectors](#combinator-selectors)
  - [Pseudo-classes](#pseudo-classes)
  - [Pseudo-element](#pseudo-element)
  - [Attribute Selectors](#attribute-selectors)
- [Typography](#typography)
  - [Text Color](#text-color)
  - [Text Alignment](#text-alignment)
  - [Text Decoration](#text-decoration)
  - [Text Transformation](#text-transformation)
  - [Text Spacing](#text-spacing)
  - [Text Shadow](#text-shadow)
  - [Font Family](#font-family)
  - [Font Size](#font-size)
  - [Font Style](#font-style)
  - [Google Font](#google-font)
  - [Icon](#icon)
  - [Cursor pointer-events and user-select](#cursor-pointer-events-and-user-select)
- [Box Model](#box-model)
  - [Box Info](#box-info)
  - [Size](#size)
  - [Background](#background)
  - [Padding](#padding)
  - [Border](#border)
  - [Outline](#outline)
  - [Margin](#margin)
  - [z-index](#z-index)
  - [Overflow](#overflow)
  - [Box Shadow](#box-shadow)
  - [Opacity](#opacity)
- [Variable](#variable)
  - [Global variable Declaration and usage](#global-variable-declaration-and-usage)
  - [Local Variable Declaration and usage](#local-variable-declaration-and-usage)
- [CSS Layout and Positioning Techniques](#css-layout-and-positioning-techniques)
  - [Float](#float)
  - [Position](#position)
  - [Display](#display)
  - [Flexbox](#flexbox)
  - [Grid](#grid)
- [Animated CSS](#animated-css)
  - [Transition](#transition)
  - [Transform](#transform)
  - [Animation](#animation)

---


## Basic CSS Structure

<img src='css structure.png'>


## CSS Type
There are three types of CSS:
<ul>
<li>Inline
<li>Internal
<li>External
</ul>

### Inline CSS
```html
<h1 style="property:value;property:value;.....">.....</h1> 
```

### Internal CSS
```html
<head>

    <style type="text/css">                                  
        h2{
            property:value;
            .......
        }
        p{
            property:value;
            .......
            
        }
    </style>

</head>

<body>

<h2>.....</h2>
<p>
    .....
</p>

</body>
```

### External CSS
```html
<head>
    <link rel="stylesheet" type="text/css" href="source of the css file">
</head>

<body>
........
.....
..
</body>
```
<b>File: </b><mark>CSS Type</mark>




## CSS Selector

<ul>

<li>Simple selectors
<ul>
<li>Tag Selector
<li>Id Selector
<li>Class Selector
<li>Universal Selector
<li>Nested Selector
<li>Multiple Selector
</ul>

<li>Combinator selectors
<ul>
<li>Descendant combinator (space)
<li>Child combinator (>)
<li>Next sibling combinator (+)
<li>Subsequent-sibling combinator (~)
</ul>

<li>Pseudo-class selectors
<ul>
</ul>

<li>Pseudo-elements selectors
<ul>
</ul>

<li>Attribute selectors
<ul>
</ul>

</ul>

### Simple Selectors

```css

/* Tag selector */
tag{
    property:value;
    .......
    
}

/* Id selector */
#id{
    property:value;
    .......
    
}
/* Class selector */
.class{
    property:value;
    .......
    
}

/* Nested selector */
#id .class tag{
    property:value;
    .......
    
}

/* Multiple selector */
p,h2{
    property:value;
    .......
    
}
```

<b>File: </b><mark>CSS Selector->simple.html</mark>

### Combinator Selectors

```css

/* Descendant combinator */
tag/#id /.class tag/#id /.class .......{
    property:value;
    ..........
}

/* Child Combinator combinator */
tag/#id /.class > tag/#id /.class {
    property:value;
    ..........
    
}

/*Next Sibling Combinator*/
tag/#id /.class + tag/#id /.class {

    property:value;
    ..........
    
}

/* Subsequent-sibling Combinator */
tag/#id /.class ~ tag/#id /.class {
    property:value;
    ..........
    
}
```

<b>File: </b><mark>CSS Selector->combinator.html</mark>

### Pseudo-classes

```css

tag/#id /.class:pseudo-class-name {
    property:value;
    ........
}
```

<b>File: </b><mark>CSS Selector->Pseudo_class.html</mark>

### Pseudo-element

```css

tag/#id /.class::pseudo-element-name {
    property:value;
    ........
}
```

<b>File: </b><mark>CSS Selector->Pseudo_element.html</mark>

### Attribute Selectors

```css

tag[attribute_name] {
    property:value;
    ........
}

tag[attribute_name="attribute value"] { /*Exact Match*/
    property:value;
    ........
}

tag[attribute_name^="attribute value"] { /*starts with*/
    property:value;
    ........
}

tag[attribute_name$="attribute value"] { /*ends with*/
    property:value;
    ........
}

tag[attribute_name*="attribute value"] { /*contains*/
    property:value;
    ........
}
```

<b>File: </b><mark>CSS Selector->attribute.html</mark>




## Typography
<ul>
<li>Text

<ul>
<li>Color
<li>Alignment
<li>Decoration
<li>Transformation
<li>Spacing
<li>Shadow
</ul>

<li>Fonts
<ul>
<li>font-family
<li>font-style
<li>font-size
<li>google font
<li>Icon
</ul>

<li>Cursor and User Interaction
<ul>
<li>Cursor
<li>pointer-events
<li>user-select
</ul>

</ul>

### Text Color

```css
selector{
    color:color_name/hex_code/rgb()/hsl();
}
```

### Text Alignment

```css
selector{
    text-align/text-align-last:left/right/center/justify;
    vertical-align:sub/super;
}
```

### Text Decoration

```css
selector{
    text-decoration-line:none/underline/overline/line-through/overline underline;
    text-decoration-color:color_name/hex_code/rgb()/hsl();
    text-decoration-style:solid/double/dotted/dashed/wavy;
    text-decoration-thickness:"25% / 5px";
}
```

### Text Transformation

```css
selector{
    text-transform:uppercase/lowercase/capitalize/none;
}
```

### Text Spacing

```css
selector{
    text-indent: 50px;
    letter-spacing: 5px;
    line-height: 0.8;
    word-spacing: 10px;
    white-space: normal/nowrap/pre/pre-line/pre-wrap;
}
```

### Text Shadow

```css
selector{
    text-shadow:x y blur color;
}
```
<b>File: </b><mark>Typography->text.html</mark>

### Font Family

```css
selector{
     font-family:value;
}
```

### Font Size

```css
selector{
    font-size:value;
}
```

### Font Style

```css
selector{
    font-weight:bold/bolder/lighter/100-900;
    font-style:normal/italic/oblique;
}
```

### Google Font

```html
<head>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap" rel="stylesheet">
</head>

<style>

    selector{
        font-family: "Poppins", sans-serif;
        font-weight: 100;
        font-style: normal;
    }

</style>
```

### Icon

```html
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@24,400,0,0&icon_names=close" />
</head>

<body>

<span class="material-symbols-outlined">
close
</span>

</body>
```
<b>File: </b><mark>Typography->font_icon.html</mark>

### Cursor pointer-events and user-select

```css

selector{
    cursor:pointer/text/grab/grabbing/no-drop/progress/wait/zoom-in/zoom-out;
    pointer-events:none;
    user-select:none;
}
```



## Box Model
<img src="box model.png">

### Box Info
<ul>
<li>Size
<ul>
<li>height
<li>max-height
<li>min-height
<li>width
<li>max-width
<li>min-width
</ul>
<li>Background
<li>Padding
<li>Borders
<li>Outline
<li>Margins
<li>z-index
<li>overflow
<li>Box Shadow
<li>Opacity
</ul>

### Size
```css
selector{
    height/width/max-height/max-width/min-height/min-width:value;
}
```
<b>File: </b><mark>Box Model->height_width.html</mark>

### Background
```css
selector{
    background-color:color_name/hex_code/rgb()/hsl();
    background-image: url("source")/linear-gradient()/radial-gradient()/conic-gradient();
    background-repeat: no-repeat/repeat-x/repeat-y;
    background-position: left/right/top/bottom/left-top/right-bottom..;
    background-attachment: scroll/fixed/local;
}
```
<b>File: </b><mark>Box Model->background.html</mark><br>
<b>File: </b><mark>Box Model->gradient.html</mark>

### Padding

```css
selector{
    padding:top right bottom left;
    padding-top/right/bottom/left:value;
    box-sizing: border-box;             /*Fixing the size width or height.
                                          padding must use*/
}
```
<b>File: </b><mark>Box Model->padding.html</mark>

### Border
```css
selector{
    border: width style color;
    border-style:dotted/dashed/solid/double/groove/ridge/inset/outset/none/hidden;
    border-top/right/bottom/left-style/color/width:dotted/dashed/solid/double/groove/ridge/inset/outset/none/hidden///color_name/hex_code/rgb()/hsl()///value;
    border-width:value;
    border-color:color_name/hex_code/rgb()/hsl();
    border-radius: value;
}
```
<b>File: </b><mark>Box Model->border.html</mark>

### Outline
```css
selector{
    outline:width style color;
    outline-style/color/width/offset:dotted/dashed/solid/double/groove/ridge/inset/outset/none/hidden///color_name/hex_code/rgb()/hsl()///value///value;

}
```
<b>File: </b><mark>Box Model->outline.html</mark>

### Margin
```css
selector{
    margin:top right bottom left;
    margin-top/right/bottom/left:value;
}
```
<b>File: </b><mark>Box Model->margin.html</mark>

### z-index

```css
selector{
    z-index:value;
}
```
<b>File: </b><mark>z-index,variable->z-index.html</mark>

### Overflow
```css
selector{
    overflow/overflow-x/overflow-y:visible/hidden/scroll/auto(scroll when needed);

}
```
<b>File: </b><mark>z-index,variable->overflow.html</mark>

### Box Shadow

```css

selector{
    box-shadow:x y blur color;
}
```

### Opacity

```css

selector{
    opacity:value from 0 to 1;
}
```


## Variable

There are two type of variable:
<ul>
<li>Local
<li>Global
</ul>

### Global variable Declaration and usage

```css
:root{
    --variable-name:value;
}

selector{
    property:var(--variable-name);
}
```

### Local Variable Declaration and usage

```css
selector{
    --variable-name:value;
    property:var(--variable-name);
}
```
<b>File: </b><mark>z-index,variable->variable.html</mark>




## CSS Layout and Positioning Techniques

### Float

```css
selector{
    float:left/right;
}

immediate selector{
    clear:left/right;
}
```
<b>File: </b><mark>Layout and Position->float.html</mark>

### Position

```css
selector{
    position:fixed/sticky/relative/absolute;
    left/right/top/bottom:value;
}
```
<b>File: </b><mark>Layout and Position->position.html</mark>

### Display
<ul>
<li>inline
<li>inline-block
<li>block
</ul>

```css
selector{
    display:inline/inline-block/block;
}
```
<b>File: </b><mark>Layout and Position->display_block.html</mark>

### Flexbox

Flex Container Properties:
<ul>
<li>display
<li>flex-direction
<li>flex-wrap
<li>flex-flow
<li>justify-content
<li>align-items
<li>align-content
</ul>

```css
selector{
    display:flex/inline-flex;
    flex-direction:row/column/row-reverse/column-reverse;
    flex-wrap:wrap/wrap-reverse;
    flex-flow:flex-direction flex-wrap;
    justify-content:flex-start/flex-end/center/space-around/space-between/space-evenly;
    align-items:flex-start/center/flex-end/stretch/baseline;
    align-content:space-between/space-around/space-evenly;

    order: 1/2/3/.....;
    flex-grow:1/2/3..;
    flex-basis: 250px;
    align-self:flex-start/flex-end/center;
}
```

### Grid

grid properties:
<ul>
<li>display
<li>grid-template-columns
<li>gap/row-gap/column-gap
<li>justify-content
<li>align-content
<li>place-content
</ul>

```css
selector{
    display:grid/inline-grid;
    grid-template-columns: auto auto auto/80px 200px 100px/1fr 1fr 1fr/repeat(3, 1fr);
    gap/row-gap/column-gap: value;
    justify-content:start/end/center/space-between/space-around/space-evenly;
    align-content:start/end/center/space-between/space-around/space-evenly;
    place-content:center;
}
```



## Animated CSS

<ul>
<li>Transition

<ul>
<li>transition-property
<li>transition-duration
<li>transition-timing-function
<li>transition-delay
<li>transition
</ul>

<li>Transform
<ul>
<li>translateX()
<li>translateY()
<li>translate()
<li>scale()
<li>rotate()
</ul>

<li>Animation
<ul>
<li>animation-name
<li>animation-duration
<li>animation-delay
<li>animation-iteration-count
<li>animation-timing-function
</ul>

</ul>


### Transition

```css
selector{
    transition-property:property-name, property-name, ...;
    transition-duration:time;
    transition-timing-function:ease/linear/ease-in/ease-out/ease-in-out;
    transition-delay:time;
    transition: property duration timing-function delay;
}
```

### Transform

```css
selector{
    transform:translateX(neg/pos)/translateY(neg/pos)/translate(neg/pos)/scale(0-2)/rotate(-360-360);
}
```

### Animation

```css
selector{
    animation-name:title;
    animation-duration: time;
    animation-delay: time;
    animation-iteration-count: 3/infinite;
    animation-timing-function: ease/linear/ease-in/ease-out/ease-in-out;
}

@keyframes title {
  from {
    attribute: value;
    ........
    ....
    ..
  }

  to {
    attribute: value;
    ........
    ....
    ..
  }
}



@keyframes title {
  0% {
    attribute: value;
    ........
    ....
    ..
  }

  50% {
    attribute: value;
    ........
    ....
    ..
  }

  100% {
    attribute: value;
    ........
    ....
    ..
  }
}
```