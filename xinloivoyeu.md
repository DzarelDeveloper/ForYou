<div align="center">

# 💌 ForYou

**A playful interactive web page for sending a simple message to someone special.**

[![HTML](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/docs/Web/HTML)
[![CSS](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)](https://developer.mozilla.org/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/docs/Web/JavaScript)
[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live-222222?logo=github)](https://dzareldeveloper.github.io/ForYou/)
[![License](https://img.shields.io/badge/License-MIT-22C55E.svg)](./LICENCE)

[Live Demo](https://dzareldeveloper.github.io/ForYou/) · [Report an Issue](https://github.com/DzarelDeveloper/ForYou/issues)

</div>

---

## About

**ForYou** is a lightweight interactive web page designed to deliver a playful confession message. The visitor is presented with a simple question and two choices:

- Selecting **Yes** changes the message and displays a new GIF.
- Moving the pointer over **No** makes the button jump to a random position on the screen.

The project is built entirely with native web technologies and does not require a framework, package manager, database, or build process.

## Preview

<div align="center">
  <img src="https://raw.githubusercontent.com/DzarelDeveloper/Img/main/gifyou.webp" alt="ForYou animated illustration" width="320">
</div>

> Open the [live demo](https://dzareldeveloper.github.io/ForYou/) to try the complete interaction.

## Features

- Interactive **Yes** and **No** choices
- Dynamic message and GIF replacement
- Random button positioning based on the browser viewport
- Lightweight implementation with no framework
- No installation or build step required
- Deployable on any static hosting service

## Built With

| Technology | Purpose |
|---|---|
| HTML5 | Page structure and interactive elements |
| CSS3 | Layout, colors, buttons, and presentation |
| JavaScript | Click handling, GIF replacement, and random button movement |

## How It Works

The JavaScript selects the question, GIF, and both buttons from the DOM.

1. When **Yes** is clicked, the question text and GIF source are updated.
2. When the pointer enters **No**, the script reads the button dimensions.
3. It calculates the available viewport area.
4. A random horizontal and vertical position is generated.
5. The button is moved to that position.

## Getting Started

### Run locally

Clone the repository:

```bash
git clone https://github.com/DzarelDeveloper/ForYou.git
cd ForYou
```

Open `index.html` directly in a browser, or start a local server:

```bash
python -m http.server 8000
```

Then visit:

```text
http://localhost:8000
```

If `python` is unavailable, try `python3`.

## Project Structure

```text
ForYou/
├── index.html     # Page structure
├── style.css      # Visual styling
├── script.js      # Interactive behavior
├── foryou.zip     # Archived project files
├── LICENCE        # MIT License
└── README.md      # Project documentation
```

## Customization

### Change the question

Edit the heading in `index.html`:

```html
<h2 class="question">You like me?</h2>
```

### Change the response

Edit the message inside the **Yes** button event in `script.js`:

```javascript
question.innerHTML = "Aaaaa, I like you too";
```

### Replace the GIFs

Update the initial GIF URL in `index.html` and the response GIF URL in `script.js`. You can use local files instead:

```text
assets/question.webp
assets/response.webp
```

Then point each `src` value to the appropriate file.

### Change the theme

The main accent color is `#e94d58`. Replace it in `style.css` to create a different color theme. You can also adjust the background, typography, button dimensions, and spacing in the same file.

## Deployment

Because this is a static project, it can be deployed using:

- GitHub Pages
- Netlify
- Vercel
- Cloudflare Pages
- Any standard web server

For GitHub Pages, publish the root of the `main` branch. No environment variables are required.

## Browser Notes

The evasive **No** button currently uses the `mouseover` event, which is designed primarily for mouse or trackpad interaction. Touch-screen behavior may vary between mobile browsers. A future improvement could add `touchstart` or pointer-event support.

The GIF files are loaded from an external GitHub repository, so an internet connection is required for those images to appear.

## Contributing

Contributions are welcome. You can open an [issue](https://github.com/DzarelDeveloper/ForYou/issues) for a bug or suggestion, or submit a pull request with a focused improvement.

Please keep the project lightweight and avoid adding dependencies unless they provide a clear benefit.

## License

This project is available under the [MIT License](./LICENCE).

## Author

Created and maintained by [DzarelDeveloper](https://github.com/DzarelDeveloper).

---

<div align="center">

**Made with HTML, CSS, JavaScript, and a little courage. ❤️**

</div>
