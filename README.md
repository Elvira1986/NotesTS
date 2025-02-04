# NotesTS

This is app build in TypeScript React

### To get your local copy, use terminal:

`git clone https://github.com/Elvira1986/NotesTS.git` - to clone this repository to your local computer;
`cd NotesTS` - get inside of the path project
`npm install` -install and manage packages (dependencies) for Node Package Manager

### To get additional packages for project:

`npm i react-bootstrap bootstrap react-router-dom` - adding bootstrap and routing dependecies
`npm i uuid` - install id

`npm run dev` - run app locally on port `http://localhost:5173/`

```js
export default tseslint.config({
  languageOptions: {
    // other options...
    parserOptions: {
      project: ["./tsconfig.node.json", "./tsconfig.app.json"],
      tsconfigRootDir: import.meta.dirname,
    },
  },
});
```

- Replace `tseslint.configs.recommended` to `tseslint.configs.recommendedTypeChecked` or `tseslint.configs.strictTypeChecked`
- Optionally add `...tseslint.configs.stylisticTypeChecked`
- Install [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) and update the config:

```js
// eslint.config.js
import react from "eslint-plugin-react";

export default tseslint.config({
  // Set the react version
  settings: { react: { version: "18.3" } },
  plugins: {
    // Add the react plugin
    react,
  },
  rules: {
    // other rules...
    // Enable its recommended rules
    ...react.configs.recommended.rules,
    ...react.configs["jsx-runtime"].rules,
  },
});
```

# NotesTS
