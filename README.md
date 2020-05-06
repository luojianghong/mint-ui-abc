# Mint UI (ABC定制版本)

> Mobile UI elements for **Vue 2.0**

- [Homepage](http://mint-ui-abc.github.io)
- [Documentation](http://mint-ui-abc.github.io/docs)



## Installation
```shell
npm i mint-ui-abc -S

# for Vue 1.x
npm i mint-ui-abc@1 -S
```

## Usage

Import all components.

```javascript
import Vue from 'vue';
import Mint from 'mint-ui-abc';
import 'mint-ui-abc/lib/style.css';

Vue.use(Mint);
```

Or import specified component. (Use [babel-plugin-component](https://www.npmjs.com/package/babel-plugin-component))

```javascript
import { Cell, Checklist } from 'mint-ui-abc';

Vue.component(Cell.name, Cell);
Vue.component(Checklist.name, Checklist);
```


Equals to

```javascript
import Vue from 'vue';
import Mint from 'mint-ui-abc';
import 'mint-ui-abc/lib/style.css';

Vue.use(Mint);

// import specified component

import MtRadio from 'mint-ui-abc/lib/radio';
import 'mint-ui-abc/lib/radio/style.css';

Vue.component(MtRadio.name, MtRadio);
```

## babel-plugin-component
- Auto import css file
- Modular import component

Installation
```shell
npm i babel-plugin-component -D
```

Usage

.babelrc
```json
{
  "plugins": ["other-plugin", ["component", [
    { "libraryName": "mint-ui-abc", "style": true }
  ]]]
}
```

## CDN

NPMCDN

- https://unpkg.com/mint-ui-abc/lib/index.js
- https://unpkg.com/mint-ui-abc/lib/style.css

## Development

```shell
npm run dev
```

## Contribution
Please make sure to read the [Contributing Guide](https://github.com/ElemeFE/mint-ui/blob/master/.github/CONTRIBUTING_en-us.md) before making a pull request.

## License
MIT
