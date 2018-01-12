# eslint-config-chernetsov

[![npm version](https://badge.fury.io/js/eslint-config-chernetsov.svg)](http://badge.fury.io/js/eslint-config-chernetsov)

This package makes little sense without either [eslint-config-airbnb](https://www.npmjs.com/package/eslint-config-airbnb) or [eslint-config-airbnb-base](https://www.npmjs.com/package/eslint-config-airbnb-base). It only extends them with promise support and other minor tweaks.

#### Usage

Requires [eslint](https://www.npmjs.com/package/eslint), [eslint-plugin-import](https://www.npmjs.com/package/eslint-plugin-import) and [eslint-plugin-promise](https://www.npmjs.com/package/eslint-plugin-promise).

1. Ensure packages are installed with correct version numbers by running:
  ```sh
  npm v eslint-config-chernetsov peerDependencies --json |
  command sed 's/[\{\},"]//g ; s/: /@/g' |
  xargs npm i -D eslint-config-chernetsov
  ```
  Which produces and runs a command like:

  ```sh
  npm i -D eslint-config-chernetsov eslint@^0.0.0 eslint-plugin-import@^0.0.0 eslint-plugin-promise@^0.0.0
  ```

2. Add `"chernetsov"` to`"extends"` array in your **.eslintrc** probably right after `"airbnb-base"` or `"airbnb"`.
