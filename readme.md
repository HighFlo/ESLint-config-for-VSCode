# ESLint config for VSCode
1. Copy `.eslintrc.json`, and `package.json` to your project
2. Install packages with:
```cmd
npm i
```
3. Eddit your VSCode settings (settings.json) to add:
```json
"[typescript]": {
  "editor.defaultFormatter": "dbaeumer.vscode-eslint"
},
"[javascript]": {
  "editor.defaultFormatter": "dbaeumer.vscode-eslint"
},
"eslint.format.enable": true,
```

###### Note
If you want to use JavaScript instead TypeScript, edit `.eslintrc.json` and replace:
```json
"extends": ["xo-typescript/space", "plugin:unicorn/all", "airbnb-base"],
```
by:
```json
"extends": ["plugin:unicorn/all", "airbnb-base"],
```
and replace
```json
"files": ["*.ts", "*.tsx"],
```
by:
```json
"files": ["*.js"],
```
