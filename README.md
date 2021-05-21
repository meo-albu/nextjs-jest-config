
# Next js - Jest config

## 𝟭. 𝗜𝗻𝘀𝘁𝗮𝗹𝗹 𝗱𝗲𝗽𝗲𝗻𝗱𝗲𝗻𝗰𝗶𝗲𝘀

```bash
npm i jest @testing-library/react @testing-library/jest-dom identity-obj-proxy
```

## 𝟮. 𝗜𝗻 𝘁𝗵𝗲 𝗿𝗼𝗼𝘁 𝗰𝗿𝗲𝗮𝘁𝗲 𝗷𝗲𝘀𝘁.𝗰𝗼𝗻𝗳𝗶𝗴.𝗷𝘀 𝗽𝗮𝘀𝘁𝗲 𝘁𝗵𝗲 𝘁𝗲𝘅𝘁 𝗳𝗿𝗼𝗺 below

```js
// 𝗷𝗲𝘀𝘁.𝗰𝗼𝗻𝗳𝗶𝗴.𝗷𝘀

module.exports = {
  testPathIgnorePatterns: ["<rootDir>/.next/", "<rootDir>/node_modules/"],
  setupFilesAfterEnv: ["<rootDir>/setupTests.js"],
  transform: {
    "^.+\\.(js|jsx|ts|tsx)$": "<rootDir>/node_modules/babel-jest",
  },
  moduleNameMapper: {
    "\\.(css|less|scss|sass)$": "identity-obj-proxy",
  }
}

```

## 𝟯. 𝗜𝗻 𝘁𝗵𝗲 𝗿𝗼𝗼𝘁 𝗰𝗿𝗲𝗮𝘁𝗲 .𝗯𝗮𝗯𝗲𝗹𝗿𝗰 𝗮𝗻𝗱 𝗽𝗮𝘀𝘁𝗲 𝘁𝗵𝗲 𝘁𝗲𝘅𝘁 𝗳𝗿𝗼𝗺 below

```bash
{
"presets": ["next/babel"]
}

```

## 𝟰. 𝗜𝗻 𝘁𝗵𝗲 𝗿𝗼𝗼𝘁 𝗰𝗿𝗲𝗮𝘁𝗲 𝘀𝗲𝘁𝘂𝗽𝗧𝗲𝘀𝘁𝘀.𝗷𝘀 𝗮𝗻𝗱 𝗽𝗮𝘀𝘁𝗲 𝘁𝗵𝗲 𝘁𝗲𝘅𝘁 𝗳𝗿𝗼𝗺 below

```js
// 𝘀𝗲𝘁𝘂𝗽𝗧𝗲𝘀𝘁𝘀.𝗷𝘀

import "@testing-library/jest-dom"

```

## 5. 𝗨𝗽𝗱𝗮𝘁𝗲 𝗽𝗮𝗰𝗸𝗮𝗴𝗲.𝗷𝘀𝗼𝗻 𝘁𝗼 𝗮𝗱𝗱 𝗮 𝘁𝗲𝘀𝘁 𝘀𝗰𝗿𝗶𝗽𝘁

```md

"test": " jest"

```

...Write your tests. :)
