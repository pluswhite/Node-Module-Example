# Node-Module-Example

## 1. Create package.json

```bash
npm init
```

## 2. Define a entry file

`entry` is a file that return object o method for the `require('your_module_name')` call.

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

1. if it's a error message that `you do not have permission to publish "your module name", Are you logged in as the correct user?`, that's mean this module had exist.
2. if you update module and want to republish, you must update your module version file in package.json.
3. your registry config must be `http://registry.npmjs.org`.
