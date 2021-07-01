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

Clone the repo into your PC.

Then, copy the `css` folder into your project directory.

Then, include the `flex-grid.min.css` file in your html file.

```html
<link rel="stylesheet" href="css/flex-grid.min.css" />
```

> **Hint:** I assume that your html file is in the root directory.

## Usage

Once you include `flex-grid.min.css` in your html file you are all set to use `flex-grid`, now just you need to add some classes.

`flex-grid` is a rows and columns grid-based, each row represents a grid system, and each column represents a grid element, each row divided into 12 grid elements that can be represented by columns.

| class      | description                                                           |
| ---------- | --------------------------------------------------------------------- |
| .container | You can use it as a container for your content.                       |
| .row       | Container of your grid elements, all grid elements must be inside it. |
| .col-\*    | Represents a grid element.                                            |
| .order-\*  | Uses for ordering your grid elements.                                 |

### .container

You can use it as a container for your content, handles the content to be all the same.

### .row

Container of your grid elements, all grid elements must be inside it.

### .col-

Represents a grid element,

> **Hint:** Consuming `flex-grid` classes is just like bootstrap framework.
