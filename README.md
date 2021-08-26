# Visual Studio Code configuration

This is a configuration process for Visual Studio Code (made for angular projects)

## Settigs

You need to override (or merge) the settings.json file of your visual with this settings.json

```
visual > ctrl+shift+p > Preferences: Open Settings (JSON)
```

Paste the content of settings.json

## Linter

If not installed you need to instal eslint

```
npm install -g eslint
```

Paste the file .eslintrc into your project root directory

If not installed you need to install a few basic linter rules

```
npm i -D eslint babel-eslint eslint-config-standard eslint-plugin-import eslint-plugin-node eslint-plugin-promise eslint-plugin-standard standard
npm i -D typescript @typescript-eslint/parser @typescript-eslint/eslint-plugin
```

If you are interested in add more rules you can check this pages
<a href="https://eslint.org/docs/rules/" class="navbar-brand"><img alt="ESLint" src="https://1.bp.blogspot.com/-RE1QxyoTpEc/XwhpVqFBm3I/AAAAAAAFH5s/T8tgKwNIIuk0zsfLAxHycE_9JSUz_ky5wCLcBGAsYHQ/s1400/eslint.png"  width="100px"></a>
<a href="https://github.com/typescript-eslint/typescript-eslint/tree/master/packages/eslint-plugin" class="navbar-brand"><img alt="ESLint" src="https://1.bp.blogspot.com/-RE1QxyoTpEc/XwhpVqFBm3I/AAAAAAAFH5s/T8tgKwNIIuk0zsfLAxHycE_9JSUz_ky5wCLcBGAsYHQ/s1400/eslint.png" width="100px"></a>

## Format

If not installed, install prettier

```
npm i -g prettier
```

Paste the .prettierignore and the .prettierrc into your project root directory

If after installing prettier the files dont format is because the prettier is not the default formatter. For making it default

```
right button on file > format document with > configure > select prettier
```

To format the whole project you could add the next script into package.json and launch

```
"prettier": "prettier \"**/*.{json,html,scss,js,ts}\" --write"
```
