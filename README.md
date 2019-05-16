# vscode 配置

## 插件
```
1、Atom One Dark Theme
2、Auto Close Tag
3、Auto Complete Tag
4、Auto Import
5、Auto Rename Tag
6、Babel ES6/ES7
7、Better Align
8、Better Comments
9、Chai snippets
10、Chinese (Simplified) Language Pack for Visual Studio Code
11、Code Spell Checker
12、Color Highlight
13、Debugger for Chrome
14、ES6 Mocha Snippets
15、ESLint
16、ExpressSnippet
17、Full React/React Native/React Router/Redux/GraphQL/ES7/18、Testing/PropTypes snippets
19、Guides
20、Identical Sublime Monokai C# theme and colorizer
21、Import Cost
22、Indenticator
23、JavaScript (ES6) code snippets
24、JS JSX Snippets
25、Live Server
26、Lodash Snippets
27、Manta's Stylus Supremacy
28、markdownlint
29、Material Icon Theme
30、Node.js Modules Intellisense
31、npm Intellisense
32、open in browser
33、Path Autocomplete
34、Path Intellisense
35、Prettier - Code formatter
36、React Native Tools
37、Vetur
38、VSCode Great Icons
39、Ant Design Vue helper
40、翻译
41、language-stylus
42、stylus
43、Highlight Matching Tag
44、Vue 2 Snippets

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
## 新建vue代码片段

>文件-->首选项-->用户代码片段-->点击新建代码片段--取名vue.json 确定。
>删除不要的代码,入自己写的.vue模板。
```
{
  "Print to console": {
      "prefix": "vue",
      "body": [
          "<!-- 页面说明 -->",
          "<template>",
          "  <div></div>",
          "</template>",
          "",
          "<script>",
          "import { mapState } from 'vuex';",
          "export default {",

          "  components: {},",
          "  data() {",
          "    return {",
          "      ",
          "    };",
          "  },",
          "  watch() {",
          "    ",
          "  },",
          "  computed:{",
          "    ...mapState({",
          "      ",
          "    })",
          "  },",
          "  created() {",
          "    ",
          "  },",
          "  mounted() {",
          "    ",
          "  },",
          "  methods: {",
          "    ",
          "  },",
          "  beforeDestroy() {",
          "    ",
          "  },",
          "}",
          "</script>",
          "",
          "<style lang='stylus' scoped>",
          "$4",
          "</style>"
      ],
      "description": "Log output to console"
  }
}


```