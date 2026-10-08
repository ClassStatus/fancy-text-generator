# fancy-text-generator
its npm package to create fancy text using this lab
# Fancy Text Generator

[Fancy Text Generator](https://www.thefancytext.com) is a Node.js module that allows you to generate fancy and stylish text using various decorative fonts and styles. Perfect for adding flair to your web app. use below keys
Bold,
Italic,
BoldItalic,
Underline,
Strikethrough,
Monospace,
Superscript,
Subscript,
Fraktur,
BoldFraktur,
Double Struck,
Script,
Bold Script,
Fancy1,
Fancy2,
Fancy3,
more to come...

## Installation

Use the package manager [npm](https://www.npmjs.com/) to install fancy text Generator.

```bash
npm install fancy-text-generator
```

## Usage

```js
const generateFancyText = require("fancy-text-generator");

const inputText = "hello world";
generateFancyText(inputText, "italic"); // returns ℎ𝑒𝑙𝑙𝑜 𝑤𝑜𝑟𝑙𝑑
generateFancyText(inputText, "bold"); // returns 𝗵𝗲𝗹𝗹𝗼 𝘄𝗼𝗿𝗹𝗱
generateFancyText(inputText, "underline"); // returns 𝒽̲𝑒̲𝓁̲𝓁̲ℴ̲ 𝓌̲ℴ̲𝓇̲𝓁̲𝒹̲
generateFancyText(inputText, "fancy1"); // returns 🅗🅔🅛🅛🅞 🅦🅞🅡🅛🅓
generateFancyText(inputText, "fancy2"); // returns 🄷🄴🄻🄻🄾 🅆🄾🅁🄻🄳
generateFancyText(inputText, "fancy3"); // returns ん乇ﾚﾚの Wの尺ﾚり
```

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)
