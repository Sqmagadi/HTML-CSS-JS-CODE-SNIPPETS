# STICKY HORIZONTAL FOOTER ICON BAR

This simple web page demonstrates how to make a Responsive Horizontal Icon Bar using HTML and CSS.

## HTML Structure

The icons are imported from **font awesome** with a link placed in the header section of the HTML file.

```html
<head>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
</head>
```

## CSS

A simple style is added to give the page a better look.

## Solution

`position: sticky;` and `bottom: 0;` keeps the bar sticky at the bottom of the view port.

```css
.icon-bar {
    width: 100%;
    background-color: var(--gray-color);
    overflow: auto;
    bottom: 0;
    position: sticky;
    z-index: 100;
}
```

<img src="images/icon-bar.png" width= "80%" height= "auto">

**Sticky Bar**

<img src="images/sticky.png" width= "80%" height= "auto">

### Break Point

A media query is used to lower the font sizes in smaller screens.

We also remove the footer.

```css
@media (max-width: 680px) {
    html {
        font-size: 13px;
    }

    .icon-bar a {
        padding: 0.1em 0;
    }

    footer {
        display: none;
    }
}
```

<img src="images/responsive.png" width= "80%" height= "auto">

## Changes

Feel free to modify the HTML and CSS files to suit your needs.

## Author

SQCODES

## License

This project is free for use any where. You do not need to get any permission to use it.