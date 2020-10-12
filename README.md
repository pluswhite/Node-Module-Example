# Node-Module-Example

![npm](https://img.shields.io/npm/v/node-module-example-of-thsi?label=npm-package)
![GitHub](https://img.shields.io/github/license/EricThsi/Node-module-example)
![npm](https://img.shields.io/npm/dm/node-module-example-of-thsi)

## 1. Create package.json

```bash
npm init
```

Note: define your module name in `name` field of `package.json`.

## 2. Define a entry file

`entry` is a file that return object method for the `require('your_module_name')` call.

Can be config in `main` field of `package.json`

## 3. login your npm account

```bash
npm login
npm whoami
```

## 4. Publish your module

```bash
npm publish
```

## 5. Install and Use your module

```bash
# Anthor directory
npm install your-package-name
```

```js
const myModule = require('your-package-name');
myModule();
```

## Notice:

1. If it occurs an error message that `you do not have permission to publish "your module name", Are you logged in as the correct user?`, that means this module had alredy existed.
2. If you update module and want to republish, you **must** update your module version file in package.json, you can use the npm cli `npm version major/minor/patch`.
3. Your registry config must be `http://registry.npmjs.org`, or you can config it a Github npm registry by `https://npm.pkg.github.com`.
