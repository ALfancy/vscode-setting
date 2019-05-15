# vscode 配置

## 插件
```
Atom One Dark Theme
Auto Close Tag
Auto Complete Tag
Auto Import
Auto Rename Tag
Babel ES6/ES7
Better Align
Better Comments
Chai snippets
Chinese (Simplified) Language Pack for Visual Studio Code
Code Spell Checker
Color Highlight
Debugger for Chrome
ES6 Mocha Snippets
ESLint
ExpressSnippet
Full React/React Native/React Router/Redux/GraphQL/ES7/Testing/PropTypes snippets
Guides
Identical Sublime Monokai C# theme and colorizer
Import Cost
Indenticator
JavaScript (ES6) code snippets
JS JSX Snippets
Live Server
Lodash Snippets
Manta's Stylus Supremacy
markdownlint
Material Icon Theme
Node.js Modules Intellisense
npm Intellisense
open in browser
Path Autocomplete
Path Intellisense
Prettier - Code formatter
React Native Tools
Vetur
VSCode Great Icons
Ant Design Vue helper

```
## 配置json

```
{
  "explorer.confirmDelete": false,
  "window.zoomLevel": 0,
  "editor.renderIndentGuides": false,
  "workbench.iconTheme": "material-icon-theme",
  "editor.fontSize": 15,
  "editor.quickSuggestionsDelay": 0,
  "files.trimTrailingWhitespace": true,
  "breadcrumbs.enabled": true,
  "editor.wordWrap": "on",
  "files.exclude": {
    "**/.git": true,
    "**/.svn": true,
    "**/.hg": true,
    "**/CVS": true,
    "**/.DS_Store": true,
    "**[表情]de_modules": true
  },
  "editor.rulers": [80, 120],
  "editor.quickSuggestions": {
    "other": true,
    "comments": true,
    "strings": true
  },
  "editor.minimap.enabled": true,
  "editor.renderWhitespace": "all",
  "editor.renderControlCharacters": false,
  "guides.active.width": 3,
  "explorer.confirmDragAndDrop": false,
  "javascript.updateImportsOnFileMove.enabled": "always",
  "workbench.colorTheme": "Sublime Monokai",
  "editor.suggestSelection": "first",
  "vsintellicode.modify.editor.suggestSelection": "automaticallyOverrodeDefaultValue",
  "git.autofetch": true,
  "workbench.startupEditor": "newUntitledFile",
  "git.confirmSync": false,
  "git.enableSmartCommit": true,
  // vscode默认启用了根据文件类型自动设置tabsize的选项
  "editor.detectIndentation": false,
  // 重新设定tabsize
  "editor.tabSize": 2,
  // #每次保存的时候自动格式化
  "editor.formatOnSave": false,
  // #每次保存的时候将代码按eslint格式进行修复
  "eslint.autoFixOnSave": true,
  // 添加 vue 支持
  "eslint.validate": [
    "javascript",
    "javascriptreact",
    {
      "language": "vue",
      "autoFix": true
    }
  ],
  //  #让prettier使用eslint的代码格式进行校验
  "prettier.eslintIntegration": true,
  //  #去掉代码结尾的分号
  "prettier.semi": false,
  //  #使用带引号替代双引号
  "prettier.singleQuote": true,
  //  #让函数(名)和后面的括号之间加个空格
  "javascript.format.insertSpaceBeforeFunctionParenthesis": true,
  // #这个按用户自身习惯选择
  "vetur.format.defaultFormatter.html": "js-beautify-html",
  // #让vue中的js按编辑器自带的ts格式进行格式化
  "vetur.format.defaultFormatter.js": "vscode-typescript",
  "vetur.format.defaultFormatterOptions": {
    "js-beautify-html": {
      "wrap_line_length": 20000,
      "wrap_attributes": "auto",
      "end_with_newline": false
      // #vue组件中html代码格式化样式
    }
  },
  // 格式化stylus, 需安装Manta's Stylus Supremacy插件
  "stylusSupremacy.insertColons": false, // 是否插入冒号
  "stylusSupremacy.insertSemicolons": false, // 是否插入分好
  "stylusSupremacy.insertBraces": false, // 是否插入大括号
  "stylusSupremacy.insertNewLineAroundImports": false, // import之后是否换行
  "stylusSupremacy.insertNewLineAroundBlocks": false,
  "[javascript]": {
    "editor.defaultFormatter": "vscode.typescript-language-features"
  },
  "[html]": {
    "editor.defaultFormatter": "vscode.html-language-features"
  } // 两个选择器中是否换行
}
```