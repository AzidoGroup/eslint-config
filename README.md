# eslint-config-azido

Azido Group [ESLint](http://eslint.org/) Rules and Standards.

## Installation within a project

Make sure you do not already have `eslint` globally installed in your system. There's an ESLint [bug report](https://github.com/eslint/eslint/issues/1877) with further details.

### Remove ESLint globally
```bash
npm uninstall eslint -g
rm ~/.eslintrc
```

Add a new `devDependencies` to your project:

```bash
npm install --save-dev git+ssh://git@github.com/AizdoGroup/eslint-config-azido
```

In the project root directory, add the file `.eslintrc.json`:

```bash
touch .eslintrc.json
```

In the `.eslintrc.json` file, add the following:

```javascript
{
  "extends": "eslint-config-azido"
}
```

## Use

Configure your editor to automatically lint all files.

See http://eslint.org/docs/user-guide/integrations to determine how to best configure your editor.

To execute ESLint directly:

```bash
./node_modules/.bin/eslint .
```

Run the script:

```bash
npm run -s eslint
```

## Further Reading

* [ESLint Shareable Configuration files](http://eslint.org/docs/developer-guide/shareable-configs)
* [ESLint Integrations](http://eslint.org/docs/user-guide/integrations)
