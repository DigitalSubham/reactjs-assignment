Theory -
● What is Emmet?

Emmet is a productivity tool for web developers that allows them to write HTML and CSS code more quickly and efficiently. 
It is a plugin that can be used with popular code editors like Visual Studio Code, Sublime Text, and Atom.

Emmet uses abbreviations to expand into HTML or CSS code. 
For example, if you type ul>li*3>a and then press the Emmet shortcut key, it will expand into:

<ul>
  <li><a href=""></a></li>
  <li><a href=""></a></li>
  <li><a href=""></a></li>
</ul>


This saves time and reduces the chances of errors when writing code. 
Emmet also has many other features, such as the ability to generate Lorem Ipsum text, create CSS rules with shorthand syntax, and more.

Emmet is widely used by web developers and is an essential tool for anyone looking to increase their productivity and efficiency when writing HTML and CSS code.


● Difference between a Library and Framework?

A library and a framework are both software development tools, but they differ in their approach to solving development problems and how they are used.

A library is a collection of reusable code that can be called upon to perform specific tasks. 
A library provides a set of functions or classes that can be called from a program to perform a specific task. 
For example, a library might provide functions for sorting arrays, parsing XML, or creating graphics.

A framework, on the other hand, is a more comprehensive set of tools and conventions that dictate the structure and organization of an application. 
A framework provides a set of rules and guidelines that developers must follow when building an application. 
It often includes libraries and tools that can be used to implement specific features or functionalities.




● What is CDN? Why do we use it?

CDN stands for Content Delivery Network. It is a system of distributed servers that deliver web content to users based on their geographic location. 
The primary purpose of a CDN is to reduce latency, improve website performance, and provide a better user experience.

When a user requests a resource (such as an image or a video) from a website, the request is routed to the nearest CDN server, rather than the origin server where the resource is hosted. 
This reduces the distance that the request needs to travel, which reduces the time it takes to load the resource.

CDNs are used for a variety of reasons, including:

Faster website performance: By delivering content from a server closer to the user, a CDN can significantly reduce the time it takes to load web pages and resources. This can result in faster page load times and a better user experience.

Scalability: CDNs can handle large amounts of traffic and distribute it across multiple servers, making it easier for websites to handle spikes in traffic and avoid downtime.

Cost-effectiveness: By offloading content delivery to a CDN, websites can reduce the load on their origin servers, which can save on bandwidth costs and reduce the need for additional infrastructure.

Global reach: CDNs have servers located all around the world, making it easier for websites to serve content to users in different geographic locations.

***How CDN Works?

The CDN server that receives the request then checks to see if it has a cached copy of the requested resource. 
If it does, it delivers the cached copy to the user's browser, which reduces the time it takes to load the resource.

If the CDN server does not have a cached copy of the requested resource, it forwards the request to the origin server where the resource is hosted. 
The origin server then sends the resource back to the CDN server, which caches the resource and delivers it to the user's browser. 
This process is known as "origin pull."

CDNs typically use a technique called "load balancing" to distribute traffic across multiple servers. 
This helps to ensure that no single server is overloaded with traffic, which can cause slow page load times and downtime.

CDNs also often use advanced caching techniques, such as edge caching and dynamic caching, to further improve performance and reduce the load on origin servers.




● Why is React known as React?
React is known as React because it is built around the concept of "reacting" to changes in a web application's user interface. 
The framework was initially developed by Facebook in 2011 for internal use and was called "FaxJS" at the time. 
It was later released to the public in 2013 under the name "React."

React uses a "virtual DOM" (Document Object Model) to represent the UI of a web application. 
The virtual DOM is a lightweight representation of the actual DOM, which allows React to quickly and efficiently update the UI in response to user interactions and other events.

When a user interacts with a React-based web application (such as clicking a button or typing in a form field), React "reacts" to the change by updating the virtual DOM, which then triggers a re-rendering of the UI. 
This process is known as "reconciliation," and it allows React to update the UI quickly and efficiently, without requiring a full page reload.

In summary, React is known as React because it is built around the concept of reacting to changes in a web application's UI. 
Its use of a virtual DOM and efficient updating mechanisms make it a popular choice for building fast, dynamic, and responsive web applications.





● What is crossorigin in script tag?

The "crossorigin" attribute in a script tag is used to specify whether the browser should allow scripts from different domains to be executed on a web page. 
It is used as a security measure to prevent cross-site scripting attacks (XSS) and to protect user data.

When a script is loaded from a different domain than the one hosting the web page, the browser considers it a "cross-origin" request. 
By default, the browser blocks scripts from being executed when they are loaded from a different origin. 
However, if the script has the "crossorigin" attribute set, the browser will allow the script to be loaded and executed 
if the server hosting the script sends the appropriate CORS (Cross-Origin Resource Sharing) headers indicating that the script is safe to use.

The "crossorigin" attribute can have three possible values: "anonymous", "use-credentials", and an empty value. 
If the attribute is set to "anonymous", the browser will not send any credentials (such as cookies or authentication tokens) with the request. 
If it is set to "use-credentials", the browser will include credentials with the request. 
If the attribute is not set or has an empty value, the browser will use its default behavior, which may vary depending on the browser.

Overall, the "crossorigin" attribute is an important security feature that helps protect web users from malicious scripts and other security threats.




● What is diference between React and ReactDOM?

React and ReactDOM are two different libraries in the React ecosystem, each with its own distinct role:

React: React is a JavaScript library for building user interfaces. It provides a declarative approach to building UIs by allowing developers to define UI components as small, reusable pieces of code. 
React uses a virtual DOM to efficiently update the UI and minimize the number of DOM manipulations needed. 
React is often used with other libraries and tools such as Redux, React Router, and Webpack.

ReactDOM: ReactDOM is a library that provides the glue between React and the browser DOM. 
It provides the necessary functionality to render React components to the browser DOM. 
ReactDOM provides several methods for rendering React components to the DOM, including render(), hydrate(), and createPortal(). 
It also provides utility functions for working with the DOM, such as findDOMNode() and unmountComponentAtNode().

In summary, React is the core library for building UI components and managing state, 
while ReactDOM is the library for rendering those components to the browser DOM. 
While they work closely together, they serve different purposes and are often used together in React applications.



● What is difference between react.development.js and react.production.js files via CDN?

The difference between the react.development.js and react.production.js files via CDN lies in how they are optimized for development and production environments, respectively.

react.development.js: This file is designed for development environments and contains additional warnings, error messages, and debugging information. 
It includes helpful features such as error messages that explain what went wrong, the location of the error, and how to fix it. 
It also includes warnings about potential performance issues, such as the use of deprecated features or inefficient code.

react.production.js: This file is optimized for production environments and is typically used in the final build of a React application that is deployed to a live website. 
It has been minified and stripped of any unnecessary code, resulting in a smaller file size and faster load times. 
It does not include the additional warnings, error messages, and debugging information that are included in the development version, as these are not needed in a production environment where performance is critical.

When using React via a CDN, it is important to use the appropriate version depending on whether you are developing or deploying a production build of your application. 
For development purposes, you would use the react.development.js file, while for production builds, 
you would use the react.production.js file to optimize performance and reduce the size of the bundle that needs to be downloaded by users.




● What is async and defer? - see my Youtube video ;)

Both the async and defer attributes are used in HTML script tags to load external scripts asynchronously and improve page loading performance. 
However, they function differently and have different use cases.

async attribute: The async attribute tells the browser to load the script asynchronously, 
meaning that it will continue loading the rest of the page while the script is being downloaded in the background. 
When the script is downloaded and parsed, it will execute immediately, even if the rest of the page is not yet fully loaded. 
This is useful for scripts that do not have any dependencies on the page's content and can run independently.

defer attribute: The defer attribute also loads the script asynchronously, 
but it waits until the entire page is finished parsing before executing the script. 
This means that the script will not block the page's rendering or slow down its loading. 
defer is useful for scripts that have dependencies on the page's content and need to be executed after the page has finished rendering.

In summary, the async attribute is best used for scripts that do not depend on the page's content and can be executed independently, 
while the defer attribute is best used for scripts that have dependencies on the page's content and need to be executed after the page has finished rendering. 
Both attributes can be used to improve page loading performance and should be chosen based on the specific needs of the script being loaded.

some use cases where you might use async or defer when loading scripts:

Use async when:
Loading third-party scripts or analytics trackers that don't affect the page's content or functionality.
Including scripts that are not essential for the page's initial rendering or interaction, but may enhance the user experience 
(e.g. social media sharing buttons, chat widgets, etc.).
Loading scripts that do not have any dependencies on other scripts or the page's content and can be executed independently.


Use defer when:
Including scripts that need to be executed after the page's content has finished loading and rendering 
(e.g. scripts that manipulate the DOM or modify the page's content).
Loading scripts that have dependencies on other scripts or the page's content and need to be executed in a specific order.
Including scripts that might cause conflicts or errors if they are executed before the page's content is fully loaded.
In general, it's a good practice to use async and defer when loading scripts to improve page loading performance and avoid blocking the page's 
rendering or interaction. However, it's important to choose the appropriate attribute based on the specific needs of the script being 
loaded and to test the page's performance and functionality after making any changes to the script loading process.








Coding -
● Set up all the tools in your laptop 
○ VS Code
○ Chrome
○ Extensions of Chrome
● Create a new Git repo


● Build your first Hello World program using, 
  ○ Using just HTML
  ○ Using JS to manipulate the DOM 
  ○ Using React
    ■ use CDN Links
    ■ Create an Element
    ■ Create nested React Elements
    ■ Use root.render
    
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Namaste Javascript</title>
  </head>
  <body>
    <div>
      <h1 id="hello">hello World</h1>
    </div>
    <div id="root">Not Rendered</div>

    <!-- manipulating using dom -->
    <script>
      document.getElementById("hello").innerHTML = "Namaste";
    </script>

<!-- using react cdn -->
    <script
      crossorigin
      src="https://unpkg.com/react@18/umd/react.development.js"
    ></script>
    <script
      crossorigin
      src="https://unpkg.com/react-dom@18/umd/react-dom.development.js"
    ></script>
    <script src="app.js"></script>
  </body>
</html>


//app.js file starts

// creating h1 elemnt using react

const heading = React.createElement(
  "h1",
  {
    id: "title",
  },
  "Heading 1"
);

//creating h2 elemnent using react

const heading2 = React.createElement(
  "h2",
  {
    id: "title", class:"title"
  },
  "Heading 2"
);

//crating div container using react which having id container 

const container = React.createElement(
  "div",
  {
    id: "container",
  },
  [heading, heading2] //nesting of elements
);

console.log(heading);

const root = ReactDOM.createRoot(document.getElementById("root"));

//passing a react element inside the root

//async defer
root.render(container); //rendering

    
