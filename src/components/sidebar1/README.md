# react-tailwind-sidebar-ts

A simple sidebar template with [React](https://react.dev/) and [Tailwind](https://tailwindcss.com/)

## Create React Project With [Vite](https://vitejs.dev/guide/)

```
npm create vite@latest react-tailwind-sidebar-ts -- --template react-ts
```
### Install libraries

```
npm install
```

### Run on development mode

```
npm run dev
```


### Testing the App Locally

```
npm run build
npm run preview
```

The vite preview command will boot up a local static web server that serves the files from dist at http://localhost:4173. It's an easy way to check if the production build looks OK in your local environment.

### Testing the App Locally with [npm serve](https://github.com/vercel/serve)

Add this script to package.json

```
"serve": "npx serve -p 4173 -s dist"
```

## Install [tailwindcss](https://tailwindcss.com/docs/guides/vite)

### Install Tailwind library

```
npm install -D tailwindcss postcss autoprefixer
```

### Init Tailwind configuration

```
npx tailwindcss init -p
```

### Edit ***tailwind.config.js***

```
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

### Edit ***src/index.css***

```
@tailwind base;
@tailwind components;
@tailwind utilities;
```

### Edit ***src/App.tsx***

```
function App() {

  return (
    <>
      <h1 className="text-3xl font-bold underline">
        Hello world!
      </h1>
    </>
  )
}

export default App
```

### Delete unused file

- src/App.css

## Install other libraries

- [clsx](https://github.com/lukeed/clsx)

  Utility for constructing className

- [Icons from](https://icons.radix-ui.com/)

  List of svg icons