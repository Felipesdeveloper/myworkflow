# myworkflow

## VS Code

### Extensions

- [Bracket Pair Colorizer](https://marketplace.visualstudio.com/items?itemName=CoenraadS.bracket-pair-colorizer);
- [Docker](https://code.visualstudio.com/docs/azure/docker);
- [EditorConfig for VS Code](https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig);
- [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint);
- [LiveServer](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
- [One Dark Pro](https://marketplace.visualstudio.com/items?itemName=zhuangtongfa.Material-theme);
- [open in browser](https://marketplace.visualstudio.com/items?itemName=techer.open-in-browser);
- [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense);
- [vscode-icons](https://marketplace.visualstudio.com/items?itemName=robertohuertasm.vscode-icons);
- [formate: CSS/LESS/SCSS formatter](https://marketplace.visualstudio.com/items?itemName=MikeBovenlander.formate);
- [todo highlight](https://marketplace.visualstudio.com/items?itemName=wayou.vscode-todo-highlight);
- [vscode-styled-components](https://marketplace.visualstudio.com/items?itemName=jpoissonnier.vscode-styled-components)

### Settings

```json
{
  "editor.autoIndent": false,
  "editor.fontSize": 16,
  "editor.formatOnPaste": false,
  "editor.tabCompletion": "on",
  "editor.tabSize": 2,
  "editor.renderWhitespace": "all",
  "editor.wordWrap": "on",
  "editor.rulers": [80, 120],
  "editor.formatOnSave": true,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  },
  "eslint.validate": [
    {
      "language": "html",
      "autoFix": true
    },
    {
      "language": "javascript",
      "autoFix": true
    },
    {
      "language": "javascriptreact",
      "autoFix": true
    },
    {
      "language": "typescript",
      "autoFix": true
    },
    {
      "language": "typescriptreact",
      "autoFix": true
    },
    {
      "language": "vue",
      "autoFix": true
    }
  ],
  "explorer.autoReveal": false,
  "files.insertFinalNewline": true,
  "files.trimTrailingWhitespace": true,
  "javascript.updateImportsOnFileMove.enabled": "always",
  "search.exclude": {
    "/node_modules": true,
    "/bower_components": true,
    "**/dist": true
  },
  "workbench.colorTheme": "One Dark Pro Darker",
  "formate.verticalAlignProperties": false,
  "workbench.sideBar.location": "right",
  "typescript.updateImportsOnFileMove.enabled": "always",
  "editor.formatOnSaveMode": "modifications",
  "bracket-pair-colorizer-2.depreciation-notice": false,
  "workbench.iconTheme": "vscode-icons"
}
```

### Snippets

```json
{
  "functional component": {
    "prefix": "rfc",
    "body": [
      "import React from 'react';",
      "",
      "interface Props {",
      "  example: string;",
      "}",
      "",
      "const ${1:Name}: React.FC<Props> = (props: Props) => <>{props.example}</>;",
      "",
      "export default ${1};",
      ""
    ]
  },
  "container component": {
    "prefix": "rcc",
    "body": [
      "import React from 'react';",
      "import { connect } from 'react-redux';",
      "import { ${1:AppStateInterface} } from '../../store';",
      "",
      "interface StateProps {",
      "  example: string;",
      "}",
      "",
      "const ${2:Name}: React.FC<StateProps> = (props: StateProps) => <>{props.example}</>;",
      "",
      "const mapStateToProps = (state: ${1}): StateProps => ({",
      "  example: state.example,",
      "});",
      "",
      "export default connect(mapStateToProps)(${2});",
      ""
    ]
  },
  "styled components": {
    "prefix": "stld",
    "body": [
      "import styled from 'styled-components';",
      "",
      "export const ${1:Name} = styled.${2:tagName}`",
      "${3}",
      "`;",
      ""
    ]
  },
  "import export component": {
    "prefix": "iexpt",
    "body": ["export { ${2:default} } from './${1:ComponentName}';", ""]
  },
  "import": {
    "prefix": "impt",
    "body": ["import {${2}} from './${1}';", ""]
  }
}
```

## Terminal

[Oh my zsh](https://github.com/robbyrussell/oh-my-zsh)

[Theme for zsh](https://github.com/denysdovhan/spaceship-zsh-theme)

### Extensões

- [zinit](https://formulae.brew.sh/formula/zinit)
- [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting/blob/master/INSTALL.md)
- [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions)
