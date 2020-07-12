# Sass config
- Editor : VSCode
- OS : Windows 10
 
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
