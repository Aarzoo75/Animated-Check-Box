# Animated Checkbox
This is a simple and customizable animated checkbox built with HTML, CSS, and JavaScript. The checkbox has a modern design that includes an animation when it is checked or unchecked.

## Usage
To use this animated checkbox, simply copy and paste the HTML and CSS code into your project. You can then customize the styling to match your project's design.

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>Animated Checkbox</title>
</head>

<body>
    <div id="checklist">
        <input id="01" type="checkbox" name="r" value="1" checked>
        <label for="01">HTML</label>
        <input id="02" type="checkbox" name="r" value="2">
        <label for="02">CSS</label>
        <input id="03" type="checkbox" name="r" value="3">
        <label for="03">JS</label>
    </div>
</body>

</html>
```

```css
#checklist {
    --background: #ffffff;
    --text: #414856;
    --check: #4F29F0;
    --disabled: #C3C8DE;
    --width: 100px;
    --height: 140px;
    --border-radius: 10px;
    background: var(--background);
    width: var(--width);
    height: var(--height);
    border-radius: var(--border-radius);
    position: relative;
    box-shadow: 0 10px 30px rgba(65, 72, 86, 0.05);
    padding: 30px 45px;
    display: grid;
    grid-template-columns: 30px auto;
    align-items: center;
}

#checklist label {
    color: var(--text);
    position: relative;
    cursor: pointer;
    display: grid;
    align-items: center;
    width: -webkit-fit-content;
    width: -moz-fit-content;
    width: fit-content;
    transition: color 0.3s ease;
}

#checklist label::before,
#checklist label::after {
    content: "";
    position: absolute;
}

#checklist label::before {
    height: 2px;
    width: 8px;
    left: -27px;
    background: var(--check);
    border-radius: 2px;
    transition: background 0.3s ease;
}

#checklist label:after {
    height: 4px;
    width: 4px;
    top: 8px;
    left: -25px;
    border-radius: 50%;
}

#checklist input[type=checkbox] {
    -webkit-appearance: none;
    -moz-appearance: none;
    position: relative;
    height: 15px;
    width: 15px;
    outline: none;
    border: 0;
    margin: 0 15px 0 0;
    cursor: pointer;
    background: var(--background);
    display: grid;
}
```

## Customization
The CSS variables can be adjusted to customize the look and feel of the animated checkbox. Here are the variables and their default values:

```css
#checklist {
    --background: #ffffff;
    --text: #414856;
    --check: #4
```
