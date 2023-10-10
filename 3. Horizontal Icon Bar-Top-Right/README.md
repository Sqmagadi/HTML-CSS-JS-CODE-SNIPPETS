# TOP HORIZONTAL ICON BAR - TOP-RIGHT

This simple web page demonstrates how to make a Responsive Horizontal Icon Bar using HTML and CSS.

## HTML Structure

The icons are imported from **font awesome** with a link placed in the header section of the HTML file.

```html
<head>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
</head>
```

## CSS

A simple style is added to give it a better look.

*"float: right"* is added to the icon bar to push it to the right.

```css
.icon-bar {
    background-color: var(--gray-color);
    overflow: auto;
    float: right;
}
```

The bar items floats next to each other from left to right

```css
.icon-bar a {
    float: left;
    text-align: center;
    color: var(--white-color);
    font-size: 2.5rem;
    padding: .5em 1em ;
    transition: all 0.4s ease;
}
```

## Solution

<img src="images/icon-bar.png" width= "80%" height= "auto">

### Break Point

A media query is used to lower the font sizes in smaller screens. The bar width is also adjusted to 100%.

```css
@media (max-width: 680px) {
    html {
        font-size: 13px;
    }

    .icon-bar {
        width: 100%;
    }

    .icon-bar a {
        padding: 0.1em 0;
        width: 25%;
    }
}
```

<img src="images/responsive.png" width= "80%" height= "auto">

## Changes

Feel free to modify the HTML and CSS files to suit your needs.

## Author

@SQCODES

## License

This project is free for use any where. You do not need to get any permission to use it.