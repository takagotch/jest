### jest
---
.js
https://github.com/facebook/jest

.java
https://github.com/searchbox-io/Jest

```
yarn add --dev jest
npm install --save-dev jest

PASS ./sum.test.js
jest my-test --notify --config=config.json
jest --init

yarn add --dev babel-jest @babel/core @babel/preset-env
```

```js
function sum(a, b){
  return a + b;
}
module.exports = sum;

const sum = require('./sum');
test('adds 1 + 2 to equal 3', () => {
  expect(sum(1, 2)).toBe(3);
});

module.exports = {
  presets: [
    [
      '@babel/preset-env',
      {
        targets: {
          node: 'current',
        },
      },
    ],
  ],
};

module.exports = api => {
  const isTest = api.env('test');
  
  return {
  };
};

module.exports = {
  transform: {},
};

import React form 'react';
import Link from '../Link.react';
import renderer from 'react-test-renderer';

it('renders correctly', () => {
  const tree = renderer
    .create(<Link page="http://www.facebook.com">Facebook</Link>)
    .toJSON();
  expect(tree).toMatchSnapshot();
});
```

```
{
  "scripts": {
    "tests": "jest"
  }
}

"dependencies": {
  "babel-core": "^6.26.3",
  "babel-jest": "^23.6.0",
  "babel-preset-env": "^1.7.0",
  "jest": ""
}
```


