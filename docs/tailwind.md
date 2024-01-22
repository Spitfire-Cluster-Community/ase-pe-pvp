# Tailwind

Tailwind is a CSS framework packed with classes like `flex` , `pt-4` , `text-center` and `rotate-90` that can be composed to build any design.

The CSS is generated on-demand as you develop html pages/templates instead of being generated in advance at initial build time. We specify content: ['./**/*.html'] in `tailwind.config.js`, the just-in-time engine scans all html files in this folder and generates the used styles into a tailwind output css file. For example, if we never used the class `m-6` in any html file then it won't be outputted into the file.

See [official Tailwind website](https://tailwindcss.com/)

## Installation

Tailwind was installed using the following:

```
yarn init -y
yarn add -D tailwindcss@latest postcss@latest autoprefixer@latest postcss-cli
yarn tailwindcss init -p
```

## Updating

Run the following to rebuild the CSS based on the used classes in the HTML:

```
npx tailwindcss -i ./github_pages/assets/css/main.css -o ./github_pages/assets/css/tailwind.css --watch
```

Note, the `--watch` option rebuilds the CSS each time the HTML changes.
