# Sass config
- Editor : VSCode
- OS : Windows 10

## Live Sass Compiler
If you use VSCode, you can install the ["Live Sass Compiler"](https://marketplace.visualstudio.com/items?itemName=ritwickdey.live-sass) extension to compile your SASS or SCSS file to CSS files.

## Install Sass
To install Sass you can follow the steps on this site : https://sass-lang.com/install  
I personnaly use Node.js so i installed Sass by typing this command :  
`npm install -g sass`

## package.json
To generate a JSON package you need to have Node.js installed then you can type the following command in a integrated terminal in VSCode :  
`npm init`  

Then, we will add 2 scripts in the scripts section in the package.json file. Here are the 2 scripts :  
`"sass-e": "sass --watch ./assets/sass/main.scss:./assets/css/application.css --style expanded"`  
`"sass-c": "sass --watch ./assets/sass/main.scss:./assets/css/application.css --style compressed"`  

Before running Sass, you will need the "node_modules" folder. This folder contain all the modules you will need to run Sass.

## Run Sass
To run Sass, follow the steps below :  
- Open an integrated terminal in VSCode
- Type this command if you want to run the first script : `npm run sass-e`
- Or type this command if you want to run the second script : `npm run sass-c`

## 7-1 Directories system
This system is very useful to order and to manage better our codebase.
The concept is simple : there are 7 directories in which we will store our code. This 7 directories are imported in 1 file called "main.scss". Only the main.scss will be converted to simple css by the script in the "package.json".

Here are the seven directories :
- Base
- Utils
- Layouts
- Components
- Pages
- Themes
- Vendors

> **Base/** contains the files that define the foundations of your website. For example the fonts or a typeface style.

> **Utils/** contains your variables, functions, mixins and the `%placeholders` for the extensions.

> **Layouts/** contains reusable code blocks. For example a header, a footer or a navbar.

> **Components/** contains more indenpendant code blocks like buttons.

> **Pages/** contains code blocks that apply to only one page.

> **Themes/** contains thematic code like for Christmas or for the summer.

> **Vendors/** contains external code.

To import a file in the "main.scss" file, use the command `@import "./utils/folderName";`

Source : https://openclassrooms.com/fr/courses/6106181-simplifiez-vous-le-css-avec-sass/6599201-utilisez-le-systeme-7-1-pour-une-codebase-plus-simple-a-gerer

In this GitHub repository you will find a batch script to create a folder tree with the 7-1 directories system integrated.