# Installation VSCode plugin

Execute ```Extensions: Install Extensions``` command from Command Palette.
Type ```@sort:installs stylelint``` into the search form and install the topmost one.

Read the [extension installation guide](https://code.visualstudio.com/docs/editor/extension-gallery) for more details.

# Optional (but recommended) setup

To prevent both [the editor built-in linters ](https://code.visualstudio.com/docs/languages/css#_syntax-verification-linting) ```[css]``` ```[less]``` ```[scss]``` and this extension ```[stylelint]``` from reporting essentially the same errors, disable the built-in ones in User or Workspace [setting](https://code.visualstudio.com/docs/getstarted/settings):

```
"css.validate": false,
"less.validate": false,
"scss.validate": false
```

# Install Prettier
Install through VS Code extensions. Search for Prettier - Code formatter

[Visual Studio Code Market Place: Prettier - Code formatter](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)

Can also be installed using

```ext install prettier-vscode```


Add following lines in User or Workspace [setting](https://code.visualstudio.com/docs/getstarted/settings):

```
"[javascript]": {
    "editor.formatOnSave": true
},
"[less]": {
    "editor.formatOnSave": true
},
"prettier.stylelintIntegration": true,
```
