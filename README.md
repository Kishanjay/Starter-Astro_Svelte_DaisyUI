# Astro Svelte TailwindCSS DaisyUI TypeScript Starter.

This repo contains a working boilerplate for an Astro project that includes Svelte, TailwindCSS, DaisyUI and TypeScript.

## ⚙️ How this project was generated

[Read the Blogpost / Full Tutorial](https://kishannirghin.medium.com/setting-up-astro-with-svelte-tailwind-daisyui-typescript-anno-may-2024-9d086af0ddcb)


### Quick breakdown

```sh
# Create package.json for keeping dependencies
npm init

# Creating a new astro project
npm create astro@latest

# Dive into the newly created folder
cd astro-starter

# Add Svelte to the astro project
npx astro add svelte

# Add Tailwind to the astro project
npx astro add tailwind

# Install the DaisyUI dependency
npm i -D daisyui@latest
```

Now make sure that DaisyUI is picked up by Tailwind, this can be done by making sure the `tailwind.config.mjs` contains atleast the following plugin.

```ts
import daisyui from "daisyui"

export default {
  //...
  plugins: [daisyui],
}
```


## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

```text
/
├── public/
│   └── favicon.svg
├── src/
│   ├── components/
│   │   └── Card.astro
│   ├── layouts/
│   │   └── Layout.astro
│   └── pages/
│       └── index.astro
└── package.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

There's nothing special about `src/components/`, but that's where we like to put any Astro/React/Vue/Svelte/Preact components.

Any static assets, like images, can be placed in the `public/` directory.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

