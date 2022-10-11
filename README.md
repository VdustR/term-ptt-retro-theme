# PTT Retro Theme

A retro theme for [term.ptt.cc](https://term.ptt.cc/) based on [term-ptt-custom-theme](https://github.com/VdustR/term-ptt-custom-theme) .

![term-ptt-retro-theme](https://vdustr.dev/asset-2022/07-11-term-ptt-retro-theme/sign-in.png)

![term-ptt-retro-theme](https://vdustr.dev/asset-2022/04-08-term-ptt-custom-theme/retro.png)

- Palette: [gruvbox.css](https://github.com/VdustR/gruvbox.css)
- Font: [Fusion Pixel Font](https://github.com/TakWolf/fusion-pixel-font) (Set [ˇ](https://unicode-table.com/en/02C7/) width to 1200)

## Usage

```js
// ==UserScript==
// @name         PTT Retro Theme
// @description  https://github.com/VdustR/term-ptt-retro-theme
// @version      0.0.0
// @match        https://term.ptt.cc/
// ==/UserScript==

(function () {
  "use strict";
  function addCss(href) {
    const link = document.createElement("link");
    link.setAttribute("rel", "stylesheet");
    link.setAttribute("href", href);
    document.body.appendChild(link);
  }
  addCss("https://cdn.jsdelivr.net/gh/vdustr/term-ptt-retro-theme/theme.css");
})();
```

It's optional to set a pixel font:

```
Fusion Pixel PTT,MingLiu,SymMingLiu,monospace
```

## License

[MIT](https://github.com/VdustR/term-ptt-custom-theme/blob/main/LICENSE) © [ViPro](https://vdustr.dev).
