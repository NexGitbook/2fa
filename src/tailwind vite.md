# Tailwind

1. 
```sh
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```

2. 
// tailwind.config.js
```js
/** @type {import('tailwindcss').Config} */
export default {
  content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

3. 
// tailwind.css
```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

4. 
```html
<h1 className="text-3xl font-bold underline">
  Hello world!
</h1>
```
