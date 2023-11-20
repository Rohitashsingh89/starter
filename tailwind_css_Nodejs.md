# Tailwind CSS Starter Kit

This is a simple guide to help you set up a basic project with Tailwind CSS.

## Prerequisites

Make sure you have the following installed on your machine:

- [Node.js](https://nodejs.org/)
- [npm](https://www.npmjs.com/) (comes with Node.js)

## Create a new project

Open your terminal and run the following commands:

```bash
# Create a new directory for your project
mkdir my-tailwind-project
cd my-tailwind-project

# Initialize a new Node.js project
npm init -y

# Install Tailwind CSS and its dependencies
npm install tailwindcss postcss autoprefixer
```

This will create a new project in a folder called `my-tailwind-project` and install Tailwind CSS and its dependencies.

## Configure Tailwind CSS

Create a file named `postcss.config.js` in your project directory and add the following content:

```javascript
module.exports = {
  plugins: {
    tailwindcss: {},
    autoprefixer: {},
  },
};
```

Create a file named `tailwind.config.js` in your project directory and run the following command to generate the default configuration:

```bash
npx tailwindcss init -p
```

## Create your styles

Create a CSS file, for example, `styles.css`, in your project directory and add the following content:

```css
@import 'tailwindcss/base';
@import 'tailwindcss/components';
@import 'tailwindcss/utilities';

/* Your additional styles go here */
```

## Build your CSS

Add a script to your `package.json` file to build your CSS:

```json
"scripts": {
  "build:css": "postcss styles.css -o public/styles.css"
}
```

Run the build script:

```bash
npm run build:css
```

This will generate a `public/styles.css` file with your compiled Tailwind CSS.

## Include the CSS in your HTML

Link the generated CSS file in your HTML file:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="public/styles.css">
  <title>Tailwind CSS Project</title>
</head>
<body>
  <!-- source tailwind css docs -->
  <figure class="md:flex bg-slate-100 rounded-xl p-8 md:p-0 dark:bg-slate-800">
  <img class="w-24 h-24 md:w-48 md:h-auto md:rounded-none rounded-full mx-auto" src="/sarah-dayan.jpg" alt="" width="384" height="512">
  <div class="pt-6 md:p-8 text-center space-y-4">
    <blockquote>
      <p class="text-lg font-medium">
        “Tailwind CSS is the only framework that I've seen scale
        on large teams. It’s easy to customize, adapts to any design,
        and the build size is tiny.”
      </p>
    </blockquote>
    <figcaption class="font-medium">
      <div class="text-sky-500 dark:text-sky-400">
        Sarah Dayan
      </div>
      <div class="text-slate-700 dark:text-slate-500">
        Staff Engineer, Algolia
      </div>
    </figcaption>
  </div>
</figure>

</body>
</html>
```

## Project Structure

The basic project structure will look like this:

```
my-tailwind-project/
|-- node_modules/
|-- public/
|   |-- styles.css
|-- styles.css
|-- package.json
|-- postcss.config.js
|-- tailwind.config.js
|-- README.md
```

- `node_modules/`: The folder containing installed npm packages.
- `public/`: The folder containing the generated CSS file.
- `styles.css`: Your main CSS file where you import Tailwind CSS.
- `package.json` and other configuration files.

## Additional Setup

Explore the [Tailwind CSS documentation](https://tailwindcss.com/docs) for more information on using different utility classes and customization options.

Happy coding with Tailwind CSS! 🚀
