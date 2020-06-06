# Neo Stack Pack

This is an extension pack used and maintained for developers at https://www.neofinancial.com/

## Preferences

Some useful preferences to add to settings.json to make everyone's lives easier:

- VSCode will often auto-import files as import something from 'src/whatever' which will work locally. In prodution, however, the code runs in a docker container and src does not exist so it will crash. This setting will tell VSCode to use relative paths for its imports: import something from '../../whatever'

```json
"javascript.preferences.importModuleSpecifier": "relative",
"typescript.preferences.importModuleSpecifier": "relative"
```

- This block will tell ESLint to lint .js, .jsx, ,ts, and .tsx files in the editor.

```json
  "eslint.validate": [
    "javascript",
    "javascriptreact",
    "typescript",
    "typescriptreact"
  ]
```

- It is handy to auto-format on file save

```json
"editor.formatOnSave": true
```

## Included Extensions:

- Editorconfig
- Trailing spaces
- Code spell checker
- Color picker
- Docker
- DotENV
- ESLint
- Git Blame
- Git History
- Github Markdown Preview
- Github Pull Requests
- gitignore
- GraphQL for VSCode
- Image preview
- Prettier
- Quit Control for VSCode
- Rainbow Brackets
- SVG Viewer
- Terraform
- Todo Tree
- Jest Runner
- drawio
