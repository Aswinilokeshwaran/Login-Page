# Login-Page
Here's a detailed explanation of the HTML and CSS code of Login Page

## Code Explanation

### HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Login</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <form>
        <h1 class="head">LOGIN</h1>
        <label>Username</label>
        <input type="text">
        <label>Password</label>
        <input type="password">
        <button>Login</button>
        <a>Forget password :(</a>
    </form>
</body>
</html>
```

- **`<!DOCTYPE html>`**: Declares the document type as HTML5, helping the browser to render the page correctly.
- **`<html lang="en">`**: Sets the language of the HTML document to English.
- **`<head>`**: Contains meta-information about the document, like the title and linked stylesheets.
  - **`<title>Login</title>`**: Sets the title of the webpage, which appears on the browser tab.
  - **`<link rel="stylesheet" href="style.css">`**: Links the external CSS file `style.css` to style the HTML elements.
- **`<body>`**: Defines the main content of the webpage.
  - **`<form>`**: Represents a form where users can enter data. It is used here to create a login form.
    - **`<h1 class="head">LOGIN</h1>`**: Displays the main heading "LOGIN" at the top of the form.
    - **`<label>Username</label>`**: Creates a label for the username field.
    - **`<input type="text">`**: Creates a text input field for the username.
    - **`<label>Password</label>`**: Creates a label for the password field.
    - **`<input type="password">`**: Creates a password input field that hides the entered characters.
    - **`<button>Login</button>`**: Creates a button labeled "Login".
    - **`<a>Forget password :(</a>`**: Displays a link to indicate forgotten passwords (though it currently doesn't link anywhere).

### CSS

```css
* {
    padding: 0;
    margin: 0;
    cursor: pointer;
}
```
- Resets the default margin and padding for all elements to ensure consistency across browsers. Also, changes the cursor to a pointer for interactive elements.

```css
.head {
    font-family: 'Segoe UI';
    text-align: center;
    text-decoration: solid;
}
```
- Applies the 'Segoe UI' font, centers the heading text, and ensures there is no underline or other text decoration.

```css
body {
    height: 100vh;
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    background: linear-gradient(to right, #6F4E37, #987070);
}
```
- Sets the body to occupy the full viewport height and width. Uses `display: flex` to center the form both vertically and horizontally. The background is a gradient transitioning from a coffee brown (`#6F4E37`) to a pinkish shade (`#987070`).

```css
form::before, form::after {
    content: " ";
    position: absolute;
    width: 200px; /* Adjusted for form::before */
    height: 200px; /* Adjusted for form::before */
    background: #987070;
    border-radius: 50%;
    z-index: -1;
    opacity: .8;
}
```
- Adds two circular background elements (`::before` and `::after`) to the form for visual enhancement. These pseudo-elements have varying positions and sizes, giving a unique style to the background.

```css
form {
    width: 25rem;
    height: 28rem;
    display: flex;
    flex-direction: column;
    box-shadow: 0 8px 32px 0 rgba(153, 154, 159, 0.37);
    border-radius: 30px;
    border-left: 1px solid rgba(255, 255, 255, 0.3);
    border-top: 1px solid rgba(255, 255, 255, 0.3);
    background-color: transparent;
}
```
- Styles the form with a fixed width and height. It uses a transparent background with soft shadows (`box-shadow`) and rounded corners (`border-radius`). The borders on the top and left sides create a subtle 3D effect.

```css
h1 {
    font-size: 50px;
    text-align: center;
    color: whitesmoke;
    text-shadow: 2px 2px 4px rgba(0, 0, 0, .2);
    letter-spacing: 2px;
    margin-bottom: 5%;
    opacity: .7;
}
```
- Styles the `h1` heading, setting the text color to `whitesmoke` and adding a subtle shadow to give depth.

```css
label {
    font-size: 20px;
    color: white;
    margin-left: 20px;
    opacity: .8;
    text-shadow: 2px 2px 4px rgba(0, 0, 0, .2);
}
```
- Applies consistent styling for the labels, including size, color, and slight shadow.

```css
input {
    width: 50%;
    margin: 5% auto;
    border: none;
    outline: none;
    background: transparent;
    border-bottom: 1px solid rgba(255, 255, 255, 0.3);
    font-family: 'Times New Roman';
}
```
- Sets the width of input fields to 50%, removes the default border and background, and adds a bottom border to create an underline effect. The `margin: auto` centers the input fields.

```css
button {
    width: 50%;
    padding: 9px;
    margin: 3% auto;
    color: white;
    font-size: 15px;
    background: rgba(255, 255, 255, 0.3);
    border: none;
    border-radius: 20px;
    box-shadow: 3px 3px 3px;
}
```
- Styles the `Login` button, giving it rounded corners, a translucent background, and a shadow effect to make it stand out.

```css
a {
    font-size: 15px;
    text-align: center;
    color: white;
    opacity: .7;
}
```
- Styles the anchor tag (`a`), setting the font size, color, and transparency. However, no link is defined for it.

## Summary

The provided code creates a modern login page with a gradient background, floating circular elements for visual interest, and a centered form with soft shadow effects. The use of pseudo-elements (`::before` and `::after`) adds decorative elements to the form, making it more visually appealing. The entire design focuses on simplicity and aesthetics, with clean input fields and a consistent color scheme.
