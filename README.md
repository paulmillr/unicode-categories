# Unicode categories
A list of unicode categories.
It could be used implement ECMAscript lexer etc.

## Installation

```bash
npm install unicode-categories
```

## Usage

```javascript
var unicode = require('unicode-categories');
// Tests if text is a valid ECMAscript identifier.
var isValidIdentifier = function(text) {
  return unicode.letter.test(text);
};
```

## Documentation
Library contains several unicode category regexps. Here's list of them:

(short name, long name: description)

- `Lu`, `upperCaseLetter`: upper case letter.
- `Ll`, `lowerCaseLetter`: lower case letter.
- `Lt`, `titleCaseLetter`: title case letter.
- `Lm`, `modifierLetter`: modifier letter.
- `Lo`, `otherLetter`: other letter.
- `Mn`, `nonSpacingMark`: non-spacing mark.
- `Mc`, `spaceMark`: space mark.
- `Nl`, `number`: number.
- `Nd`, `decimal`: decimal.
- `Pc`, `punctuationConnector`: punctuation connector.
- `letter`: combines `upperCaseLetter`, `lowerCaseLetter`, `titleCaseLetter`,
`modifierLetter`, `otherLetter` and `number`. `letter` is a valid js identifier.

## License
(The MIT License)

Copyright (c) 2011 Paul Miller <paulmillr@me.com>

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the 'Software'), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

