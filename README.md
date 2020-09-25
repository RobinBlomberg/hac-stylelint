# HAC Stylelint

## Installation

```
npm install --save-dev @robinblomberg/stylelint-config-hac-stylelint
```

## Configuration

Create a file called **.stylelintrc.json** at your project root:

```json
{
  "extends": "@robinblomberg/stylelint-config-hac-stylelint"
}
```

## NPM scripts

Add the following scripts to your package.json:

```json
{
  "scripts": {
    "lint-stylesheets": "npx stylelint \"src/**/*.{css,scss}\"",
    "lint-stylesheets-fix": "npx stylelint \"src/**/*.{css,scss}\" --fix"
  }
}
```

Adjust the paths according to your project/file structure as necessary (e.g. `"npx stylelint \"src/**/*.scss\""`).

To run a script, enter the following in your command line:

```
npm run lint-stylesheets
```

## Fix-on-save in VS Code

To enable Stylelint fix-on-save, add the following to your VS Code settings.json:

```json
{
  "editor.codeActionsOnSave": {
    "source.fixAll.stylelint": true
  }
}
```
