# Tailwind Layout

# Installation
To install tailwind run the following command.
```
yarn add tailwindcss
```
We need something to process our CSS through a chain of postCSS plugins. 
```
yarn add postcss-cli
```
Tailwind doesn't include any vendor prefixes. So we install one.
```
yarn add autoprefixer
```
In order to configure tailwind lets run
```
npx tailwind init
```
the above command will create tailwind.config.js file with empty values.

we will create another file `postcss.config.js` to specify which plugins we are going to use. 

Create a file `css/tailwind.css` and specify the @tailwind directives. 

add script to package.json to process the CSS through postCSS plugins. This will generate an output file. 

Run the following command to generate CSS.
```
yarn run build
```

this action will generate a CSS in the directory specified in package.json. Include the output CSS file in html.
