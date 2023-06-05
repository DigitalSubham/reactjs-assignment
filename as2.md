# Theory Assignment:
● - What is `NPM`?
Npm is a package manager which is used for managing javascript packages, it comes with node.js when we install nodejs, it comes with it. 
There is not offical name for npm but everyone mainly calls it node package manager. It contains a vast collection of pre-written code packages that developers can utilize in their own projects. 
These packages include reusable modules, libraries, frameworks, and tools, which help developers save time and effort by not having to write everything from scratch.

## Here's a breakdown of the key aspects of NPM:

Package Management: NPM allows developers to easily install, update, and remove packages for their projects. It automatically handles the dependencies between packages, ensuring that all required code is downloaded and available for use.

Publishing and Sharing: NPM provides a straightforward method for developers to publish their own packages, making them accessible to others. This encourages collaboration and allows developers to contribute to the open-source community.

Versioning: NPM manages versions of packages, allowing developers to specify the exact version they want to use in their projects. This ensures consistency and avoids unexpected bugs that might arise from using different versions of the same package.

Scripts and Commands: NPM enables developers to define custom scripts and commands in a configuration file called "package.json". These scripts can be used to automate various tasks like running tests, building the project, or starting a local server.

● - What is `Parcel/Webpack`? Why do we need it?
Parcel, webpack both are bundler which helps in making the application more efficient They serve the purpose of taking multiple modules and assets from your project, processing them, and creating optimized bundles that can be easily served to web browsers.
In this journey of namate react i am using parcel bundler.
features of bundler and why we need to use them

Alone react and react dom cant create a perfect application for that we need bundler.
there are many features that a bundler provides and due to that we use them in our project.

1. Hot Module Reloding/Replacement => It keeps the track of what we are changing in our code, and it renders only that much of code. it uses file watcher algoritm for tracking(written in c++)
2. Tree Shaking => when we install library in our project, there are lots of function our library, but we need some of them in our project, so parcel removes unused function from our app.
3. creates a mini server for our app in local machine.
4. minify the code.
5. optimise the code
6. parcel is zero confif
7. bundling of the code
8. caching while development
9. compression of code
10. compatible with older veersions
11. and many more

● - What is `.parcel-cache`
The .parcel-cache directory is a cache folder created by Parcel bundler. 
When you use Parcel to build or bundle your project, it performs various transformations, optimizations, and caching operations to generate the final output. 
The .parcel-cache directory is where Parcel stores cached data to speed up subsequent builds.


● - What is `npx` ?


● - What is difference between `dependencies` vs `devDependencies`

● - What is Tree Shaking?
when we install library in our project, there are lots of function our library, but we need some of them in our project, 
so parcel removes unused function from our app.

● - What is Hot Module Replacement?
It keeps the track of what we are changing in our code, and it renders only that much of code. 
it uses file watcher algoritm for tracking(written in c++)

● - List down your favourite 5 superpowers of Parcel and describe any 3 of them in your own words.
1. Hot Module Reloding/Replacement => It keeps the track of what we are changing in our code, and it renders only that much of code. it uses file watcher algoritm for tracking(written in c++)
2. Tree Shaking => when we install library in our project, there are lots of function our library, but we need some of them in our project, so parcel removes unused function from our app.
3. creates a mini server for our app in local machine.
4. minify the code.
5. optimise the code
6. parcel is zero confif
7. bundling of the code
8. caching while development
9. compression of code
10. compatible with older veersions
11. and many more

● - What is `.gitignore`? What should we add and not add into it?

● - What is the difference between `package.json` and `package-lock.json`

● - Why should I not modify `package-lock.json`?

● - What is `node_modules` ? Is it a good idea to push that on git?

● - What is the `dist` folder?


● - What is `browserlists`


Read about dif bundlers: vite, webpack, parcel
● Read about: ^ - caret and ~ - tilda
● Read about Script types in html (MDN Docs)
