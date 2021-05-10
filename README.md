<div align="center">
  
# Kopiert

[![Node CI](https://github.com/BetaHuhn/kopiert/workflows/Node%20CI/badge.svg)](https://github.com/BetaHuhn/kopiert/actions?query=workflow%3A%22Node+CI%22) [![Release CI](https://github.com/BetaHuhn/kopiert/workflows/Release%20CI/badge.svg)](https://github.com/BetaHuhn/kopiert/actions?query=workflow%3A%22Release+CI%22) [![GitHub](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/BetaHuhn/kopiert/blob/master/LICENSE) ![David](https://img.shields.io/david/betahuhn/kopiert)

Kopiert (copies) text to the clipboard in the browser

</div>

## 👋 Introduction

It's quite simple, include [kopiert](https://github.com/BetaHuhn/kopiert) in your site and start copying text to the clipboard.

## 🚀 Get started

### Script tag

Add this to your HTML page:

```html
<script src="https://cdn.jsdelivr.net/npm/kopiert/dist/kopiert.min.js"></script>
<script>
    kopiert.toClipboard('This text will be copied to your clipboard') // For example on a button press
</script>
```

### NPM

Install [kopiert](https://github.com/BetaHuhn/kopiert) using NPM:

```sh
npm install kopiert
```

Then add the following JavaScript code:

```javascript
import kopiert from 'kopiert'

kopiert.toClipboard('This text will be copied to your clipboard')
```

Both methods will copy the specified text to the users clipboard.

## 📖 Examples

### On button click

```html
<p id="text">This text will be copied to your clipboard.</p>
<button id="btn">Copy text</button>

<script src="https://cdn.jsdelivr.net/npm/kopiert/dist/kopiert.min.js" ></script>
<script>
    document.getElementById('btn').addEventListener('click', function() {
        const text = document.getElementById('text').textContent
        kopiert.toClipboard(text)
    })
</script>
```

## 💻 Development

- run `yarn lint` or `npm run lint` to run eslint.
- run `yarn build` or `npm run build` to produce a minifed version in the `dist` folder.

## ❔ About

This project was developed by me ([@betahuhn](https://github.com/BetaHuhn)) in my free time. If you want to support me:

[![Donate via PayPal](https://img.shields.io/badge/paypal-donate-009cde.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=394RTSBEEEFEE)

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/F1F81S2RK)

## 📄 License

Copyright 2021 Maximilian Schiller

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
