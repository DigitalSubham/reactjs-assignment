# Theory Assignments


## What is JSX?
JSX stands for JavaScript XML. JSX is nothing but html like syntax, which we can use code easily, 
As we write react.createElemnet code that is very tough to red and write but using JSX it made it easier.
At the end JSX is React Element

JSX allows us to write HTML elements in JavaScript and place them in the DOM without any createElement() and/or appendChild() methods. 
JSX makes it easier to write and add HTML in React. JSX converts HTML tags into react elements.

JSX => React.createElement => object => HTML(Dom)

### Example

**Without JSX**
```
const Heading = React.createElement{"h1", {id: "h"}, "Heading 1"}
```

**With JSX**
```
const Heading = <h1>Heading 1</h1>
```

## Superpowers of JSX
- Make Developing experience better
- Syntactical Sugar
- Readability
- Less code
- maintainability
- No Reoeatition
- Security
- Using JSX, you can write markup inside Javascript, providing you with a superpower to write logic and markup of a component inside a single .jsx file. 
  JSX is easy to maintain and debug.
  
 ### Example
 
 ```
 function greeting(user) {
//JSX
  return <h1>{user}, How are you!!!</h1>;
}
```


## Role of type attribute in script tag? What options can I use there?
The type attribute specifies the type of the script. The type attribute identifies the content between the <script> and </script> tags. 
It has a Default value which is “text/javascript”.

### type attribute can be of the following types:
text/ecmascript : this value indicates that the script is following the EcmaScript standards.
module: This value tells the browser that the script is a module that can import or export other files or modules inside it.
text/babel : This value indicates that the script is a babel type and required bable to transpile it.
text/typescript: As the name suggest the script is written in TypeScript.


## {TitleComponent} vs {<TitleComponent/>} vs {<TitleComponent></TitleComponent>} in JSX

The Difference is stated below:

{TitleComponent}: This value describes the TitleComponent as a javascript expression or a variable. The {} can embed a javascript expression or a variable inside it.
<TitleComponent/> : This value represents a Component that is basically returning Some JSX value. In simple terms TitleComponent a function that is returning a JSX value. A component is written inside the {<  />} expression.
<TitleComponent></TitleComponent> : <TitleComponent /> and <TitleComponent></TitleComponent> are equivalent only when < TitleComponent /> has no child components. The opening and closing tags are created to include the child components.

### Example

```
<TitleComponent>
    <FirstChildComponent />
    <SecondChildComponent />
    <ThirdChildComponent />
</TitleComponent>
```



# Coding Assignment:

## Create a Nested header Element using React.createElement(h1,h2,h3 inside a div with class “title”) Create the same element using JSX

**using React.createElement**
```
const head = React.createElement(
  "div", //This is react elemnet
  {
    className: "title",
  },
  [
    React.createElement("h1", {}, "heading h1"),
    React.createElement("h2", {}, "heading h"),
    React.createElement("h3", {}, "heading h3"),
  ]
);
```

**using JSX**
```
const head = (
  <div className="title">
    <h1>Heading h1</h1>
    <h2>Heading h2</h2>
    <h3>Heading H3</h3>
  </div>
);
```

## Create a functional component of the same with JSX

```
const Head = () => (
  <div className="title">
    <h1>Heading h1</h1>
    <h2>Heading h2</h2>
    <h3>Heading H3</h3>
  </div>
);
```


## Pass attributes into the tag in JSX
```
const Head = () => (
  <div className="title">
    <h1 style={{ color: "red" }}>Heading h1</h1>
    <h2 style={{ fontSize: "100px" }}>Heading h2</h2>
    <h3 style={{ border: "10px solid red" }}>Heading H3</h3>
  </div>
);
```
## Composition of Component(Add a component inside another)

```
const Head = () => (
  <div className="title">
    <h1 style={{ color: "red" }}>Heading h1</h1>
    <h2 style={{ fontSize: "100px" }}>Heading h2</h2>
    <h3 style={{ border: "10px solid red" }}>Heading H3</h3>
  </div>
);

const Test = () => (
  <div>
    <Head />
    {"Namaste React"}
  </div>
);
```

## {TitleComponent} vs {<TitleComponent/>} vs {<TitleComponent></TitleComponent>} in JSX 

```
const element = <h4>This is h4</h4>; 
const Head = () => (
  <div className="title">
    <h1 style={{ color: "red" }}>Heading h1</h1>
    <h2 style={{ fontSize: "100px" }}>Heading h2</h2>
    <h3 style={{ border: "10px solid red" }}>Heading H3</h3>
  </div>
);

const Test = () => (
  <div>
    {element}
    <Head />
    <Head></Head>
    {"Namaste React"}
  </div>
);

```


## Create a Header Component from scratch using Functional Components with JSX
- Add a Logo on left
- Add a search bar in middle Add User icon on right
- Add CSS to make it look nice

**App.js**
```
const Search = () => (
  <div>
    <input
      className="search"
      type="text"
      placeholder="Search anything you want..."
    ></input>
    <button className="btn">Search</button>
  </div>
);

const User = () => (
  <div>
    <img className="user" alt="user" src={userIcon} />
  </div>
);

const HeaderComponent = () => (
  <div className="header">
    <Logo />
    <Search />
    <User />
  </div>
);
```
**App.css**
```
.header {
  margin-top: 20px;
  display: flex;
  justify-content: space-between;
}

.logo {
  width: 300px;
  height: 50px;
  margin-top: 35px;
  margin-left: 10px;
}
.user {
  width: 60%;
  height: 100px;
  justify-content: center;
  margin-right: 50px;
  border-radius: 50%;
}

.search {
  width: 200px;
  height: 20px;
  margin-right: 10px;
  border: 3px solid black;
  margin-top: 35px;
}
.btn {
  height: 25px;
  border-radius: 10px;
  color: white;
  background: skyblue;
  font-weight: 900;
}
```


