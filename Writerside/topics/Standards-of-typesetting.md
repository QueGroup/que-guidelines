# Frontend Guidelines

## HTML

The following tags are used to build the structure of the web application:
- ```<header>``` - used to include the webpage header.
- ```<main>``` - denotes the main content of the document.
- ```<footer>``` - defines the footer or bottom part of the page.
- ```<article>``` - used to group content that is critically important for the application.
- ```<section>``` - applied to group thematically related content.

for other blocks or react components you should use ```<div>```

## CSS (SCSS)

Sass is used as the style preprocessor. Styles are organized into modules for React components, which means using ```.module.scss``` files with node-sass.

Also you should use mixins and variables for optimizing the file structure and you should save them into the ```mixins.scss``` and ```variables.scss``` respectively (in main ```src``` directory)

All styles should show the main meaning of the block. For example:

```Javascript
const MyComponent = () => {
    return (
        <div className={styles.animalsBlock}>
            <h2>Some text about animals<h2>
        <div>
    )
}
```

## TypeScript

The project employs TypeScript for strict typing to avoid errors, such as when passing properties to React components. TypeScript provides more reliable code through static typing.

## React

React components are organized into various folders based on their functional areas. For example, all components used in the header should be placed in a folder named header, where the file header.tsx contains all the components for that area. Style files are also located directly alongside the files where they are used.

```
components
|__ Header
    |__Header.tsx
    |__Header.module.scss
```

All important imports or imports from node_modules should be higher than style imports or other imports

```Javascript
    import {UseState, UseEffect} from "react"
    import styles from 'component.module.scss'
    
    const MyComponent = () => {
        ...
    }
```

## Redux

Redux is used to manage the application state. The project includes a separate redux folder where redux slicers, reducers, and other components related to state management are located.

```
redux
|__slices
|__store.js
```

Don't use redux for simple programs/applications. Instead, it's better to use Context API or regular inheritance through component props.

## Image Placement

All images (except SVG files) should be optimized to reduce file size. All images are located in the img folder, which in turn is located in the root directory public.

Here is an example folder and file structure for ease of perception:

```
public/
    └── img/
        └── example.jpg
        └── example.png
src/
    └── components/
        └── header/
            └── header.tsx
            └── header.module.scss
            └── ...
```