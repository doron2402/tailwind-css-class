# tailwind-css-class
A tutorial I've created for teaching kids the basic of css

## Steps
1. Install node modules 
```bash
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init
```
2. Add Tailwind to your CSS:
```css 
/* styles.css */
@tailwind base;
@tailwind components;
@tailwind utilities;
```
3. 	Configure Content Paths:
```js
// tailwind.config.js
module.exports = {
  content: ["./src/**/*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};
```
4. Build Your CSS:
```bash
npx tailwindcss -i ./styles.css -o ./output.css --watch
```
