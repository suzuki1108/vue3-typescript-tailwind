# vue3-typescript-tailwind

### Vue CLIの導入（初回のみ）

```jsx
$ npm install -g @vue/cli
```

### プロジェクトの作成

```jsx
$ vue create vue3-typescript-tailwind
vue 3, router, linter/prettier, babel TypeScriptを選択
```

### Tailwind CSSの導入

```jsx
$ cd vue3-typescript-tailwind
$ vue add tailwind
```

tailwindをプロジェクトのCSSに追加

`./src/index.css`を追加して、ここにtaildwindのスタイルを追加する。

```jsx
@tailwind base;
@tailwind components;
@tailwind utilities;
```

このファイル内容を`./src/main.ts`に代入する。

```jsx
import { createApp } from "vue";
import App from "./App.vue";
import router from "./router";
import './index.css'

createApp(App).use(router).mount("#app");
```


## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
