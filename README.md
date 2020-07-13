#Tailwind CSS

## Setup & Install

- npm init -y
- npm install tailwindcss postcss-cli autoprefixer
- npx tailwind init

## Init

- postcss.config.js

```
  module.exports = {
  plugins: [
  require('tailwindcss'),
  require('autoprefixer')
  ]
}
```

- css/tailwind.css

  ```
  @tailwind base;
  @tailwind components;
  @tailwind utilities;

  ```

- Config file package.json
  ```
  build": "postcss css/tailwind.css -o public/build/tailwind.css
  ```
  - npm run build
