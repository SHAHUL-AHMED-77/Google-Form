# Google Form

This repository contains a simple, responsive Google Form built with HTML and CSS. The form collects user information including name, email, age, status, source of referral, known programming languages and frameworks, and additional comments.

To ensure your images show correctly in the GitHub preview, double-check the following steps:

1. **Verify File Paths:** Ensure the paths to your images are correct relative to the `README.md` file. For example, if your images are in a folder named `images` in the root of your repository, the paths should be `images/one.png` and `images/two.png`.

2. **File Names and Extensions:** Ensure the image files are named exactly as referenced, including the correct file extension (e.g., `.png`, `.jpg`).

3. **Commit Images:** Ensure the image files are committed and pushed to the GitHub repository along with the `README.md` file.

4. **Check Case Sensitivity:** File names are case-sensitive, so ensure the case matches exactly.

Here is your updated `README.md` with these considerations:

```markdown
# Google Form

This repository contains a simple, responsive Google Form built with HTML and CSS. The form collects user information including name, email, age, status, source of referral, known programming languages and frameworks, and additional comments.

## Preview

![Form Preview](resultimages/one.png)

![Form Preview](resultimages/two.png)

## Table of Contents

- [Usage](#usage)
- [HTML Structure](#html-structure)
- [CSS Styling](#css-styling)
- [Customizations](#customizations)
- [Contributing](#contributing)
- [License](#license)

## Usage

1. **Clone the repository:**

```bash
git clone https://github.com/SHAHUL-AHMED-77/Google-Form.git
cd Google-Form
```

2. **Open the HTML file:**

   Open `index.html` in your preferred web browser to see the form in action.

## HTML Structure

The HTML file (`index.html`) includes a form that captures user details:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Google Form</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h2>GOOGLE FORM</h2>
        <form action="#" method="POST">
            <label for="name">Name:</label><br>
            <input type="text" id="name" name="name" placeholder="Enter your Name" aria-label="Enter your name"><br>

            <label for="email">Email:</label><br>
            <input type="email" id="email" name="email" placeholder="Enter your Email" aria-label="Enter your email"><br>

            <label for="age">Age:</label><br>
            <input type="number" id="age" name="age" placeholder="Enter your Age" aria-label="Enter your age"><br>

            <div class="sel">
                <label for="status">Which option best describes you?</label><br>
                <select id="status" name="status" aria-label="Select your status">
                    <option value="student">Student</option>
                    <option value="teacher">Teacher</option>
                    <option value="parent">Parent</option>
                    <option value="other">Other</option>
                </select><br>
            </div>

            <div class="hear">
                <label for="heard">How did you hear about us?</label><br>
                <input type="radio" id="advertisements" name="heard" value="advertisements">
                <label for="advertisements">Advertisements</label><br>
                <input type="radio" id="friends" name="heard" value="friends">
                <label for="friends">Friends</label><br>
                <input type="radio" id="poster" name="heard" value="poster">
                <label for="poster">Poster</label><br>
            </div>

            <div class="lang">
                <label for="languages">Languages and Frameworks Known (Check all that apply):</label><br>
                <input type="checkbox" id="html" name="languages" value="html">
                <label for="html">HTML</label><br>
                <input type="checkbox" id="java" name="languages" value="java">
                <label for="java">Java</label><br>
                <input type="checkbox" id="css" name="languages" value="css">
                <label for="css">CSS</label><br>
                <input type="checkbox" id="javascript" name="languages" value="javascript">
                <label for="javascript">JavaScript</label><br>
                <input type="checkbox" id="django" name="languages" value="django">
                <label for="django">Django</label><br>
                <input type="checkbox" id="react" name="languages" value="react">
                <label for="react">React</label><br>
                <input type="checkbox" id="angular" name="languages" value="angular">
                <label for="angular">Angular</label><br>
            </div>

            <label for="comments">Comments:</label><br>
            <textarea id="comments" name="comments" rows="7" cols="50"></textarea><br>

            <div class="sub">
                <input type="submit" value="Submit">
            </div>
        </form>
    </header>
</body>
</html>
```

## CSS Styling

The CSS file (`style.css`) styles the form to be visually appealing and responsive:

```css
@import url('https://fonts.googleapis.com/css2?family=Lato:ital,wght@0,100;0,300;0,400;0,700;0,900;1,100;1,300;1,400;1,700;1,900&family=Orbitron:wght@400..900&display=swap');

body {
    font-family: "Lato", sans-serif;
    margin: 0;
    padding: 0;
    background: url("bg.jpg") no-repeat center;
    background-size: cover;
    height: 100%;
    width: 100%;
}

h2 {
    text-align: center;
    color: #fffafa;
    font-size: 50px;
    text-shadow: #000000 5px 3px;
}

form {
    max-width: 550px;
    margin: 0 auto;
    padding: 30px 20px;
    background-color: transparent;
    border-radius: 8px;
    border: 1px solid rgb(0, 0, 0);
    box-shadow: 5px 10px 5px 5px rgba(0, 0, 0, 0.1);
}

label {
    font-weight: bold;
    color: rgb(255, 255, 255);
    margin: 10px 0;
    font-size: 20px;
    text-shadow: 2px 2px black;
}

input[type="text"],
input[type="email"],
input[type="number"],
textarea {
    width: 100%;
    padding: 10px;
    margin: 10px 0;
    border: 1px solid #000000;
    border-radius: 4px;
    box-sizing: border-box;
    background-color: #E0B0FF;
}

input::placeholder {
    color: #000000;
}

.sel {
    margin: 10px 0;
}

select {
    width: 100%;
    padding: 8px;
    border: 1px solid #ccc;
    border-radius: 4px;
    box-sizing: border-box;
    background-color: #E0B0FF;
    margin: 10px 0;
}

input[type="radio"],
input[type="checkbox"] {
    margin-right: 7px;
}

input[type="submit"] {
    background-color: #000000;
    color: rgb(0, 0, 0);
    padding: 10px 20px;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    text-align: center;
    background-color: #FBAED2;
    font-size: 16px;
}

input[type="submit"]:hover {
    background-color: #5e1271;
    color: #ffffff;
}

input[type="submit"]:focus {
    outline: none;
}

.hear {
    margin: 10px 0;
}

.hear label {
    font-size: 16px;
    line-height: 1.5;
}

.lang {
    margin: 10px 0;
}

.lang label {
    font-size: 16px;
    line-height: 1.5;
}

.sub {
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 10px 0;
}

@media (max-width: 770px) {
    form {
        max-width: 60%;
    }

    h2 {
        font-size: 30px;
    }

    label {
        font-size: 16px;
    }
}
```

## Customizations

You can customize the form by modifying the HTML and CSS files. For example, you can:

- Change the background image by replacing `bg.jpg` with your desired image.
- Adjust the color scheme by modifying the CSS styles.
- Add or remove form fields by editing the HTML structure.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

## License

This project is licensed