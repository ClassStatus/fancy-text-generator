# fancy-text-generator

Turn plain text into Unicode styles — 𝗯𝗼𝗹𝗱, 𝑖𝑡𝑎𝑙𝑖𝑐, 𝔣𝔯𝔞𝔨𝔱𝔲𝔯, 𝓈𝒸𝓇𝒾𝓅𝓉, 🅑🅤🅑🅑🅛🅔 and more — in Node.js, with no dependencies.

The output is ordinary Unicode text, not a font, so it keeps its style when pasted into Instagram bios, Discord names, TikTok captions, X posts, chat apps and anywhere else that accepts text.

This is the library version of **[TheFancyText — Fancy Text Generator](https://www.thefancytext.com/)**, where you can try 300 styles in the browser.

[![npm version](https://img.shields.io/npm/v/fancy-text-generator.svg)](https://www.npmjs.com/package/fancy-text-generator)
[![license](https://img.shields.io/npm/l/fancy-text-generator.svg)](LICENSE)

## Installation

```bash
npm install fancy-text-generator
```

## Usage

```js
const generateFancyText = require("fancy-text-generator");

generateFancyText("hello world", "bold");          // 𝗵𝗲𝗹𝗹𝗼 𝘄𝗼𝗿𝗹𝗱
generateFancyText("hello world", "italic");        // ℎ𝑒𝑙𝑙𝑜 𝑤𝑜𝑟𝑙𝑑
generateFancyText("hello world", "script");        // 𝒽𝑒𝓁𝓁ℴ 𝓌ℴ𝓇𝓁𝒹
generateFancyText("hello world", "fraktur");       // 𝔥𝔢𝔩𝔩𝔬 𝔴𝔬𝔯𝔩𝔡
generateFancyText("hello world", "fancy1");        // 🅗🅔🅛🅛🅞 🅦🅞🅡🅛🅓
```

The function takes the text and a style key, and returns a string. An unknown key returns the text unchanged.

## Styles

Keys are **case-sensitive** — write them exactly as below.

| Key | Example (`hello world`) |
|---|---|
| `bold` | 𝗵𝗲𝗹𝗹𝗼 𝘄𝗼𝗿𝗹𝗱 |
| `italic` | ℎ𝑒𝑙𝑙𝑜 𝑤𝑜𝑟𝑙𝑑 |
| `script` | 𝒽𝑒𝓁𝓁ℴ 𝓌ℴ𝓇𝓁𝒹 |
| `fraktur` | 𝔥𝔢𝔩𝔩𝔬 𝔴𝔬𝔯𝔩𝔡 |
| `monospace` | 𝗁𝖾𝗅𝗅𝗈 𝗐𝗈𝗋𝗅𝖽 |
| `underline` | 𝒽̲𝑒̲𝓁̲𝓁̲ℴ̲ 𝓌̲ℴ̲𝓇̲𝓁̲𝒹̲ |
| `strikethrough` | h̶e̶l̶l̶o̶ w̶o̶r̶l̶d̶ |
| `superscript` | ᴴᴱᴸᴸᴼ ʷᴼᴿᴸᴰ |
| `subscript` | ʰₑₗₗₒ ʷₒᵣₗᵈ |
| `fancy1` | 🅗🅔🅛🅛🅞 🅦🅞🅡🅛🅓 |
| `fancy2` | 🄷🄴🄻🄻🄾 🅆🄾🅁🄻🄳 |
| `fancy3` | ん乇ﾚﾚの Wの尺ﾚり |

Good to know:

- Letters are converted in lowercase, so `"Hello"` and `"hello"` give the same result.
- Digits, spaces and punctuation are passed through unchanged.
- Some styles use characters that older phones or games cannot display; `bold`, `italic` and `script` are the most widely supported.

## Need more styles?

The website has 300 styles, plus tools for specific uses:

- [Fancy Text Generator](https://www.thefancytext.com/) — every style at once
- [Font Generator](https://www.thefancytext.com/font-generator) — copy-and-paste fonts
- [Cursive Font Generator](https://www.thefancytext.com/cursivefontgenerator)
- [Bold Text Generator](https://www.thefancytext.com/bold-text-generator)
- [Instagram Font Generator](https://www.thefancytext.com/instagram-font-generator)
- [Developer documentation](https://www.thefancytext.com/developer-documentation) — the HTTP API and integration notes

## A note on accessibility

Screen readers often read styled characters one by one or by their Unicode names, and search engines treat `𝗵𝗲𝗹𝗹𝗼` and `hello` as different words. Use styled text for decoration, and keep anything people need to read or find in plain text.

## Contributing

Pull requests are welcome. For larger changes, please open an issue first to discuss what you would like to change.

## License

ISC
