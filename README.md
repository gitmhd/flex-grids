# flex-grid

A lightweight CSS grid system uses for making responsive websites.

## Features

-  Pure CSS.
-  Lightweight Just 8 Kilobytes.
-  Easy To Install.
-  Easy To Use.
-  Use Flexbox.
-  Great For Multilanguage Websites. <!-- NEED -->

## Installation

Clone the repo in your PC.

Then, copy the `css` folder into your project directory.

Then, include the `flex-grid.min.css` file in your html file.

```html
<link rel="stylesheet" href="css/flex-grid.min.css" />
```

> **Hint:** I assume that your html file is in the root directory.

## Usage

Once you include `flex-grid.min.css` in your html file you are all set to use `flex-grid`, now just you need to add some classes.

`flex-grid` is a rows and columns grid-based, each row represents a grid system, and each column represents a grid element, each row divided into 12 grid elements that can be represented by columns.

| Class      | Description                                                           |
| ---------- | --------------------------------------------------------------------- |
| .container | You can use it as a container for your content.                       |
| .row       | Container of your grid elements, all grid elements must be inside it. |
| .col-\*    | Represents a grid element.                                            |
| .order-\*  | Uses to order your grid elements.                                     |

### .container

You can use it as a container for your content, handles the content to be all the same.

### .row

Container of your grid elements, all grid elements must be inside it.

### .col-\*

Represents a grid element.

```html
<div class="container">
   <div class="row">
      <div class="col">1</div>
      <div class="col">2</div>
      <div class="col">3</div>
      <div class="col">4</div>
   </div>
</div>
```

Now all the elements will be the same width and fit the row.

You can add after hyphen number from 1 to 12 represents how many grid will take from the 12 grids.

```html
<div class="container">
   <div class="row">
      <div class="col-3">1</div>
      <div class="col-3">2</div>
      <div class="col-3">3</div>
      <div class="col-3">4</div>
   </div>
</div>
```

All items have the same width because I gave each column 3 grids, so the sum is 12.

You can add after hyphen breakpoints(sm, md, lg, xl) depending on the screen you target.

```html
<div class="container">
   <div class="row">
      <div class="col-1">1</div>
      <div class="col-sm-2">2</div>
      <div class="col-md-3">3</div>
      <div class="col-lg-3">4</div>
      <div class="col-xl-3">5</div>
   </div>
</div>
```

**col-1:** Targets all the screens.

**col-sm-2:** Targets the screens from 576px and above.

**col-md-3:** Targets the screens from 768px and above.

**col-lg-3:** Targets the screens from 992px and above.

**col-xl-3:** Targets the screens from 1200px and above.

### .order-\*

Uses to order your grid elements since grids are 12 so `order-*` are 12, so they will cover all grid elements.

```html
<div class="container">
   <div class="row">
      <div class="col-6 order-2">1</div>
      <div class="col-6 order-1">2</div>
   </div>
</div>
```

Accepts all the breakpoints that `.col-*` accepts.

```html
<div class="container">
   <div class="row">
      <div class="col-md-6 order-md-2">1</div>
      <div class="col-md-6 order-md-1">2</div>
   </div>
</div>
```

> **Hint:** Consuming `flex-grid` classes is just like bootstrap framework.

## Breakpoints

Here are what widths are breakpoints target.

| Breakpoint  | Description                 |
| ----------- | --------------------------- |
| .col        | For all widths.             |
| .col-**sm** | For widths 576px and above. |
| .col-**md** | For widths 768px and above. |
| .col-**lg** | For widths 992px and above. |
| .col-**xl** | For widths 1200 and above.  |

## Support

Thank you for using `flex-grid` if you experienced any issue feel free to describe it [here](https://github.com/gitmhd/flex-grid/issues).
