# AspNetCoreWebpack

This project is a template for using ASP.NET Core with Webpack and ES6 Modules.  
This architecture allows you to use the power of Webpack with any type of ASP.NET Core project.  
It can easily be extended to support eg, TypeScript, Vue.js or whatever else you want.

This template implements the following front-end features:
* ES transpiling (Using Babel)
* Nullish Coalescing Operator (Using Babel plugin)
* Optional Chaining (Using Babel plugin)
* Code splitting (Using Babel plugin and Webpack SplitChunks)
* SCSS support (Defaults to extracting to separate SCSS file)
* CSS Modules (By using ```.module.scss``` suffix)
* Lazy loading CSS/SCSS (By using ```.lazy.scss``` suffix)
* Injecting CSS/SCSS (By using ```.scss?inject``` query string)
* PostCSS support
* Autoprefixer
* Image optimizations
* Dev server (No physical files are written in development)
* Hot Module Replacement
* Cache busting
* JS linting (Using ESLint)
* CSS/SCSS linting (Using StyleLint)
* Auto formatting (Using Prettier)
* Editorconfig
* Sourcemaps

Install npm packages with ```npm install``` in project folder.  
Start development server using ```npm start``` in project folder.  
Build production files using ```npm run build``` in project folder.  
Lint project using ```npm run lint``` in project folder.  
Auto format project using ```npm run format``` in project folder.

The resulting bundles can be analyzed using ```npm run analyze``` in project folder.

Everything front-end related resides in the ```Assets``` folder in the project root, and/or in the root of ```Areas```, check out those folders for examples.

Bundles will be built for folders under ```pages``` and ```views``` that matches an MVC view or Razor page.  
Bundles will not be built for partial MVC views and Razor pages (files starting with a underscore).

The layout view will automatically figure out if a bundle exists for a page and include it if it does.
