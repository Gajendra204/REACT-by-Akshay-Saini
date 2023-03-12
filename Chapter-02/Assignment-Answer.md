#What is 'NPM'??
Answer- NPM is short for node package manager, an online directory that contains the various already registered open-source packages. NPM modules consume the various functions as a third-party package when installed into an app using the NPM command npm install .

#What is `Parcel/Webpack`? Why do we need it?
Answer-A module bundler is a tool that takes pieces of JavaScript and their dependencies and bundles them into a single file, usually for use in the browser. You may have used tools such as Browserify, Webpack, Rollup or one of many others. because we cant write anything for all things in code than we use parcel that we can minimize our code and parcel have many dependecies. it helps our code to be make faster and easy. 

HMR (Hot Module Replacement) - parcel keeps track of file changes via file watcher algorithm and renders the changes in the files
File watcher algorithm - made with C++
Minification
Cleaning our code
DEV and production Build
Super fast building algorithm
Image optimization
Caching while development
Compresses
Compatible with older version of browser
HTTPS in dev
Port Number
Consistent hashing algorithm
Zero Configuration
Automatic code splitting

#What is `.parcel-cache?
Answer- cache folder (or . parcel-cache in parcel v2) stores information about your project when parcel builds it, so that when it rebuilds, it doesn't have to re-parse and re-analyze everything from scratch. It's a key reason why parcel can be so fast in development mode.

#What is `npx` ?
Answer-NPX stands for Node Package eXecute. It is simply an NPM package runner. It allows developers to execute any Javascript Package available on the NPM registry without even installing it.

#What is difference between `dependencies` vs `devDependencies`?
Answer- Dependency is an object that contains the library, which your project requires for production environments and functioning effectively. devDependencies are those packages in the package. json file that you need only for project development purposes. Example- Babel, Webpack, etc.

#What is Tree Shaking?
Answer- Tree shaking is process of removing the unwanted code that we do not use while developing the application. In computing, tree shaking is a dead code elimination technique that is applied when optimizing code.

#What is Hot Module Replacement?
Answer- Hot Module Replacement (HMR) exchanges, adds, or removes modules while an application is running, without a full reload. 

#What is `.gitignore`? What should we add and not add into it?
Answer - gitignore file tells Git which files to ignore when committing your project to the GitHub repository. gitignore is located in the root directory of your repo. / will ignore directories with the name.

#What is the difference between `package.json` and `package-lock.json`?
Package.json-
This file is mandatory for every project
It contains basic information about the project
Application name/version/scripts

package-lock.json`-
his file is automatically generated for those operations where npm modifies either the node_module tree or package-json.
It is generated after an npm install
It allows future devs & automated systems to download the same dependencies as the project.
it also allows to go back to the past version of the dependencies without actual ‘committing the node_modules folder.
It records the same version of the installed packages which allows to reinstall them. Future installs wll be capable of building identical description tree.

#Why should I not modify package-lock.json?
Answer- package-lock.json file contains the information about the dependencies and their versions used in the project. Deleting it would cause dependencies issues in the production environment. So don't modify it, It's being handled automatically by NPM.

#What is node_modules ? Is it a good idea to push that on git?
Answer - node_modules folder like a cache for the external modules that your project depends upon. When you npm install them, they are downloaded from the web and copied into the node_modules folder and Nodejs is trained to look for them there when you import them (without a specific path). Don't push node_modulesin github because it contains lots of files(more than 100 MB), it will cost you memory space.

#What is the dist folder?
Answer - The /dist folder contains the minimized version of the source code. The code present in the /dist folder is actually the code which is used on production web applications. Along with the minified code, the /dist folder also comprises of all the compiled modules that may or may not be used with other systems.

#What is browserslist?
Answer - Browserslist is a tool that allows specifying which browsers should be supported in your frontend app by specifying "queries" in a config file. It's used by frameworks/libraries such as React, Angular and Vue, but it's not limited to them.

#Read about: ^ - caret and ~ - tilde?
Answer- caret-- 
	-Used for Compatible with version.
    -It will update you to all future minor/patch versions, without incrementing the major version. ^2.3.4 will use releases from 2.3.4 -to <3.0.0
    -It gives you backwards-compatible new functionality as well.
    -It will update to its latest version in numbers.
    -Used by NPM as default notation.

    Tilde--
    -Used for Approximately equivalent to version.
    -It will update you to all future patch versions, without incrementing the minor version. ~1.2.3 will use releases from 1.2.3 to <1.-It gives you bug fix releases.
    -It will update in decimals.
    -Not a default notation used by NPM.