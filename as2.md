# Theory Assignment:
## What is `NPM`?
Npm is a package manager which is used for managing javascript packages, it comes with node.js when we install nodejs. 
There is no offical name for npm but everyone commanly calls it node package manager. It contains a vast collection of pre-written code packages that developers can utilize in their own projects. 
These packages include reusable modules, libraries, frameworks, and tools, which help developers save time and effort by not having to write everything from scratch.

### Here's a breakdown of the key aspects of NPM:

Package Management: NPM allows developers to easily install, update, and remove packages for their projects. It automatically handles the dependencies between packages, ensuring that all required code is downloaded and available for use.

Publishing and Sharing: NPM provides a straightforward method for developers to publish their own packages, making them accessible to others. This encourages collaboration and allows developers to contribute to the open-source community.

Versioning: NPM manages versions of packages, allowing developers to specify the exact version they want to use in their projects. This ensures consistency and avoids unexpected bugs that might arise from using different versions of the same package.

Scripts and Commands: NPM enables developers to define custom scripts and commands in a configuration file called "package.json". These scripts can be used to automate various tasks like running tests, building the project, or starting a local server.

## What is `Parcel/Webpack`? Why do we need it?
Parcel, webpack both are bundler which helps in making the application more efficient They serve the purpose of taking multiple modules and assets from your project, processing them, and creating optimized bundles that can be easily served to web browsers.
In this journey of namate react i am using parcel bundler.

- **features of bundler and why we need to use them**

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

## What is `.parcel-cache`
The .parcel-cache directory is a cache folder created by Parcel bundler. 
When you use Parcel to build or bundle your project, it performs various transformations, optimizations, and caching operations to generate the final output. 
The .parcel-cache directory is where Parcel stores cached data to speed up subsequent builds.


## What is `npx` ?

NPX is a tool that comes with Node.js, which is a popular platform for running JavaScript code. NPX helps you run JavaScript programs or npm modules that are packaged and shared by other developers.

Before NPX, if you wanted to use a specific tool, you had to install it on your computer. But sometimes, installing tools globally caused problems because different tools might need different versions of the same software, which could lead to conflicts.

With NPX, you can now run these tools without installing them permanently. NPX automatically finds and runs the tool you need, and if it's not already installed, NPX temporarily installs it just for that one use.

For example, instead of installing a package globally and then running it, you can use NPX to run it directly:

> npx package-name




## What is difference between `dependencies` vs `devDependencies`?
In the context of npm (Node Package Manager) and package.json files used in Node.js projects, there is a distinction between dependencies and devDependencies. These two sections specify different types of dependencies that a project may have.

Dependencies: The dependencies section lists the packages that are required for the application to run correctly in production. These packages are necessary for the application's core functionality. When you install the project's dependencies using npm install or yarn install, the packages listed under dependencies will be installed.

DevDependencies: The devDependencies section lists the packages that are only needed during development. These packages are not required for the production version of the application to function properly. They typically include tools, libraries, or testing frameworks used for development, build processes, testing, or other development-specific tasks. Examples include testing frameworks like Jest or development server tools like nodemon. When you run npm install or yarn install with the --dev flag, the packages listed under devDependencies will be installed.

The main difference between the two is that dependencies are essential for the application to work in production, while devDependencies are only necessary for development purposes. This separation allows for better optimization and ensures that only necessary packages are included when deploying the application.

During deployment or when distributing your application to a production environment, it is common practice to exclude devDependencies from the final build to minimize the package size and avoid including unnecessary tools or libraries.

To summarize:

dependencies: Required packages for the application to run in production.
devDependencies: Development-specific packages not needed in production, used for development and build processes.
Both dependencies and devDependencies are defined in the package.json file and are managed by npm or yarn to install the necessary packages for your project based on their respective sections.

## What is Tree Shaking?
when we install library in our project, there are lots of function our library, but we need some of them in our project, 
so parcel removes unused function from our app.

## What is Hot Module Replacement?
It keeps the track of what we are changing in our code, and it renders only that much of code. 
it uses file watcher algoritm for tracking(written in c++)

## List down your favourite 5 superpowers of Parcel and describe any 3 of them in your own words.
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

## What is `.gitignore`? What should we add and not add into it?
The .gitignore file is used in Git to tell it which files and folders it should ignore and not include when you commit changes to a repository. It helps prevent certain files from being accidentally added to the repository.

Here's what you should add to a .gitignore file:

Generated files: Files that are automatically created during development, like compiled code or logs.

Dependencies: Files or folders that contain the code libraries or packages your project depends on. These are usually installed separately and don't need to be stored in the repository.

Sensitive information: Files or folders that contain private or secret data, like passwords or API keys. You don't want this information to be visible to others in the repository.

Editor-specific files: Files that your code editor creates for its own use, like settings or temporary files. These files are specific to your editor and don't need to be shared.

Operating System files: Hidden or system-specific files that your operating system creates and are not relevant to your project.

And here's what you should not add to a .gitignore file:

Source code files: Your actual code files should not be ignored. Git is meant to track changes in your code, so you want these files to be included.

Shared configuration files: If your project relies on configuration files that are important for everyone working on the project, they should not be ignored. These files should be included in version control.

Remember to regularly review and update your .gitignore file to make sure you're ignoring the right files and folders while including the necessary ones in your repository.


## What is the difference between `package.json` and `package-lock.json`?

The package.json file is for specifying the project's metadata and listing the required dependencies, while the package-lock.json file is automatically generated and locks down the specific versions of the dependencies installed in your project. It ensures that everyone working on the project has the same set of dependencies installed, reducing the risk of compatibility issues.

Both files play crucial roles in managing dependencies, with package.json defining the dependency requirements and package-lock.json ensuring consistent installations.

## Why should I not modify `package-lock.json`?
The package-lock.json file manually modify is not advised for a few simple reasons:

Consistency: The package-lock.json file helps keep everyone working on the project on the same page. It ensures that everyone has the same versions of the installed packages. Modifying it can lead to inconsistencies and make it harder for others to work on the project.

Automatic generation: The package-lock.json file is created automatically by the package manager when you install or update dependencies. It keeps track of the exact versions of packages installed. If you change it manually, you might end up with conflicts or unexpected issues.

Dependency resolution: The package manager uses the information in package-lock.json to resolve dependencies and make sure everything works together. If you modify the file, it can cause problems like incompatible package versions or missing dependencies.

Collaboration and version control: The package-lock.json file is usually shared with others working on the project through version control. If you manually modify it, it can create conflicts with their versions and cause difficulties when collaborating.

To update or manage dependencies, it's best to use the appropriate commands provided by the package manager, like **npm install** or yarn add/remove. These commands will automatically update the package-lock.json file for you, ensuring that everything stays consistent and works smoothly for everyone involved.


## What is `node_modules` ? Is it a good idea to push that on git?

node_modules is a directory that contains all the dependencies (or packages) required by a project. When you install packages using tools like npm or Yarn, they get stored in the node_modules directory. These packages consist of the code necessary for your project to function correctly.

In general, it is not recommended to push the node_modules directory to a Git repository. There are a few reasons for this:

Large size: The node_modules directory can be quite large, especially for projects with many dependencies. Pushing it to Git can significantly increase the repository size and make cloning and pulling the repository slower for other users.

Unnecessary duplication: Since the node_modules directory contains the installed packages, it essentially duplicates the information that is already specified in the package.json file. This redundancy can be avoided by using the package.json file and a package manager like npm or Yarn.

Instead of pushing node_modules to Git, it is recommended to include a package.json file and a package-lock.json or yarn.lock file. These files specify the dependencies and their exact versions required for the project. When someone clones the repository, they can use the package manager to install the required packages based on the information in these lock files.

By including the lock files, you ensure that everyone working on the project installs the exact same versions of the dependencies, which helps maintain consistency and avoids compatibility issues.



## What is the `dist` folder?

The dist folder is where you put the final version of your code that is ready to be used or deployed. It contains optimized and compressed files that are smaller in size and faster to load. This folder is created by running a process called "building" or "compiling" your code, which prepares it for actual use. The dist folder helps keep your project organized and separates the development code from the version that is ready to be shared or put into production.

## What is `browserlists`?

When we put browser lists in our package.json file. we tell our app to must run on these browsers.
> "browserslist":[ "last 2 versions"]
when we write above command then our project will support 74% of the browsers. This browserslist package comes with parcel.


Read about dif bundlers: vite, webpack, parcel
● Read about: ^ - caret and ~ - tilda
● Read about Script types in html (MDN Docs)


# Project Assignment:

 In your existing project
## intialize `npm` into your repo
To initialize npm we use this command 
> npm init in our terminal.

## install `react` and `react-dom`
To install recat and reac-dom we use 
> npm install or i react react-dom

## remove CDN links of react
To remove CDN links we have to go in index.html file then remove scripts tag that contain CDN Links

## install parcel
To install parcel we can use the command 
> npm install -D or --save-dev parcel

## ignite your app with parcel
To ignite app with parcel we use command
> npx parcel index.html

# add scripts for “start” and “build” with parcel commands
We have to add scripts in package.json file
> "start": "parcel index.html",
> "build": "parcel build index.html"

## add `.gitignore` file


## add `browserlists`

To add bowserslist in our app use this code in package.json file
> "browserslist":[ "last 2 versions"]


## build a production version of your code using `parcel build`
To build production version of our code we can use this command
> npm build or npx parcel build index.html
