# Angular Starter Kit

This is a simple guide to help you set up a basic Angular project.

## Prerequisites

Make sure you have the following installed on your machine:

- [Node.js](https://nodejs.org/)
- [npm](https://www.npmjs.com/) (comes with Node.js)
- [Angular CLI](https://angular.io/cli) (install globally)

Install the Angular CLI using the following command:

```bash
npm install -g @angular/cli
```

## Create a new Angular project

Open your terminal and run the following commands:

```bash
# Create a new Angular project
ng new my-angular-app
cd my-angular-app
```

This will create a new Angular app in a folder called `my-angular-app` and navigate into that folder.

## Serve the Angular app

Inside your project folder, run:

```bash
ng serve
```

This will start the development server, and you can access your Angular app at [http://localhost:4200](http://localhost:4200).

## Project Structure

The basic project structure will look like this:

```
my-angular-app/
|-- e2e/
|-- src/
|   |-- app/
|   |   |-- app.component.html
|   |   |-- app.component.css
|   |   |-- app.component.spec.ts
|   |   |-- app.component.ts
|   |   |-- app.module.ts
|-- angular.json
|-- package.json
|-- README.md
```

- `e2e/`: End-to-End testing folder.
- `src/`: Contains your Angular application code.
- `angular.json`: Angular configuration file.
- `package.json`: Defines your project dependencies and scripts.

## Additional Setup

You might want to explore other tools and libraries to enhance your Angular development experience:

- [Angular Material](https://material.angular.io/): A Material Design component library for Angular.
- [NgRx](https://ngrx.io/): State management for Angular applications.
- [RxJS](https://rxjs.dev/): Reactive Extensions library for JavaScript.

Happy coding with Angular! 🅰️🚀
