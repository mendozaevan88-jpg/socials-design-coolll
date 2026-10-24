# Evan — guitar covers & socials

A single-page personal site for Evanescence "Evan" Mendoza: guitar covers, social links and photos. It's one self-contained HTML file with no build step and no dependencies.

## Features

- Full-screen sections that snap into place as you scroll, with smooth scrolling
- Headline words that slide up out of a mask when the page loads
- A glowing orb with spinning chrome rings that moves between sections and tilts toward the cursor
- A purple burst animation drawn on a `<canvas>`, with intro text that lights up word by word
- Social links that slide and change color on hover
- Responsive layout down to phone size
- Respects the `prefers-reduced-motion` setting, with keyboard focus outlines on links

## Run it locally

1. Download or clone this repository.
2. Open `index.html` in any modern browser.

The page loads two fonts (Marcellus and Jost) from Google Fonts, so it needs an internet connection to show them. Without one it falls back to Georgia and your system sans-serif.

## Publish with GitHub Pages

1. Push `index.html` to a GitHub repository.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, pick your main branch and the `/ (root)` folder, then save.
4. Your site will be live at `https://<your-username>.github.io/<repository-name>/` after a minute or two.

## Customize

Everything lives in `index.html`.

| To change | Look for |
| --- | --- |
| Colors | The `:root` variables at the top of the `<style>` block (`--vio` is the purple accent) |
| Text and links | The `<section>` blocks in the `<body>` |
| Photos | The `const I = {...}` object near the bottom. Each image is embedded as base64, so replace the data string or point it at a file path such as `"photos/me.jpg"` |
| Burst intensity | The particle loop in the `draw()` function |
| Orb positions per section | The `P` array, in the order x, y, scale, rotation, opacity |

## Credits

- Layout and motion inspired by the "Smooth Scroll Snap" website demo from Coding With Ujjwal. This is an independent recreation. No code, models or footage from that site are used.
- Fonts: [Marcellus](https://fonts.google.com/specimen/Marcellus) and [Jost](https://fonts.google.com/specimen/Jost), both under the SIL Open Font License.

## License

The code is released under the [MIT License](LICENSE).

The photos embedded in the page are personal photos of the site owner and are **not** covered by the MIT License. All rights reserved. Please don't reuse them without permission. If you fork this project, replace them with your own.
