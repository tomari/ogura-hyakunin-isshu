# ogura-hyakunin-isshu

[![CircleCI](https://circleci.com/gh/tomari/ogura-hyakunin-isshu.svg?style=svg)](https://circleci.com/gh/tomari/ogura-hyakunin-isshu)

Ogura Hyakunin Isshu (小倉百人一首) is a classical Japanese anthology of one hundred Japanese waka by one hundred poets (see https://en.wikipedia.org/wiki/Ogura_Hyakunin_Isshu ).
This package is a JSON structurized version of those poems and its author metadata.
The pronunceation is also embedded in the JSON for easy integration with voice interfaces.

## Usage

### Node.js

```
npm install ogura-hyakunin-isshu
```

```
const hyakunin=require('ogura-hyakunin-isshu');
console.log(hyakunin[0].text.join(' '));
```

## Structure

```
[
  {
    "n": 1,
    "text": ["秋の田の","かりほの庵の","苫をあらみ","我が衣手は","露にぬれつつ"],
    "ruby": ["あきのたの","かりほのいほの","とまをあらみ","わがころもでは","つゆにぬれつつ"],
    "author": {"name": "天智天皇","ruby": "てんじてんのう"}
  },
  ...
]
```

## License

Probably they're all public domain, every author has deceased like 800 years ago or so.

