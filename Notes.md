# Differentiate between Real DOM and Virtual DOM.
          

> DOM is something which  you see on the screen is objectified model. DOM is nothing but the real DOM

>Virtual DOM is a virtual representation of the real DOM.It is like a lightweight copy of the actual DOM.

> In real DOM whenever there  is a change in state of a component the whole DOM gets re rendered or updated.

> In Virtual DOM  if any element gets updated  then only the jsx perticular element is updated not the whole DOM.

>Manipulating the real DOM is slow. Manipulating the virtual DOM is much faster, because nothing gets drawn onscreen

> Expensive to do DOM manipulation in real DOM, high wastage of memory storage  in real DOM.

> DOM manipulation is very easy in virtual DOM and no memory wastage  

# What is React? What are its features

React is an open-source frontend JavaScript library which is used for building
user interfaces especially for single page applications. It is used for handling view
layer for web and mobile apps. React was created by Jordan Walke, a software
engineer working for Facebook.

Features of React:
1. JSX (JavaScript Syntax Extension)
2. Virtual DOM
3. One-way data binding
4. Performance
5. Extensions
6. Conditional statements
7. Components
8. Simplicity

## JSX(JavaScript Syntax Extension): 
JSX is a combination of HTML and
JavaScript. You can embed JavaScript objects inside the HTML elements. JSX is
not supported by the browsers, as a result Babel compiler trans compile the
code into JavaScript code. JSX makes codes easy and understandable. It is
easy to learn if you know HTML and JavaScript.

## Virtual DOM:
>React uses Virtual DOM exists which is like a lightweight copy of the actual DOM(a virtual representation of the DOM. 

>So for every objectthat exists in the original DOM, there is an object for that in React Virtual DOM. It is exactly the same, but it does not have the power to directly change the layout of the document.

>Manipulating DOM is slow, but manipulating
Virtual DOM is fast as nothing gets drawn on the screen. So each time there is a change in the state of our application, virtual DOM gets updated first
instead of the real DOM.

>In real DOM whenever there is a change in state of a component the whole DOM is updated. 
In Virtual DOM if any element gets updated then only the JSX particularelement is updated not the whole DOM.

## One-way Data Binding: 
One-way data binding, the name itself says that it is a one-direction flow. The data in react flows only in one direction i.e. the data is transferred from top to bottom i.e. from parent components to child components. The properties(props) in the child component cannot return the data to its parent component but it can have communication with the parent components to modify the states according to the provided inputs. This is the working process of one-way data binding. This keeps everything modular and fast.

## Performance: 
As we discussed earlier, react uses virtual DOM and
updates only the modified parts. So , this makes the DOM to run faster. DOM
executes in memory so we can create separate components which makes the
DOM run faster.

## Components: 
React.js divides the web page into multiple components as it
is component-based.
## Simplicity: 
React.js is a component-based which makes the code reusable
and React.js uses JSX which is a combination of HTML and JavaScript. This
makes code easy to understand and easy to debug and has less code.

React is used for handling the view layer for web and mobile apps. React also allows us to
create reusable UI components. ... React allows developers to create large web
applications that can change data, without reloading the page. The main purpose of
React is to be fast, scalable, and simple.

# SPA Model

SPA stands for Single Page Application. It is a very common way of programming websites these days. The idea is that the website loads all the HTML/JS the first time you visit. When you then navigate, the browser will only rerender the content without refreshing the website.

Basically SPA stands for single page application. If a user clicks on any button from the navigation bar of a website and that website navigates to a different web page i. e. only update the page without reloading the browser's page, then that application is known as single page application.

# Bable

Babel is an inbuild transpiler that converts the ECMA Script 6 code to an ECMA Script 5 code because the browser cannot read JSX which is not a regular JavaScript object. So Babel helps to convert the JSX file to a regular JavaScript object and then pass it to the browser.

# Advantages of React over vue and angular

>In summary, React JS is better than Angular or Vue JS because of its superior Virtual DOM capabilities, its robust community support, rich documentation, its light-weight attributes, manageable learning curve, and its flexibility to allow mobile functionality with React Native’s.

>React has many benefits over Angular like quick and efficient, an additional benefit of JSX, flexibility in building blocks, isomorphic JavaScript, support of the large community, and many more.

# Library vs Framework

>Libraries in programming languages are collections of prewritten code that users can use to optimize tasks.

>A framework in programming is a tool that provides ready-made components or solutions that are customized in order to speed up development. A framework may include a library, but is defined by the principle of inversion of control (IoC). With traditional programming, the custom code calls into the library to access reusable code. With IoC, the framework calls on custom pieces of code when necessary.

>A framework is used for building and deploying an application quickly. When we use a framework, we can use resources to facilitate faster development and a greater user experience. A library is used to enhance the functionality of an application. If we develop our own library, we can use the functions in many applications.

It is very common to confuse the term framework and library, as both are tools used within programming. In fact, as described above in the section “What is a Framework?,” a library is just one tool available within a framework.

A framework is your structure or environment to build your software: it contains access to various tools, including libraries, to assist in your build.

A library is a set of low-level components that can be invoked (called) for a specific outcome. You can access a library directly, called from the code, or a framework can supply access to libraries and call out to the code (inversion of control).

# What is JSX


JSX stands for JavaScript XML.

JSX allows us to write HTML in React.

JSX makes it easier to write and add HTML in React.

 JSX(JavaScript Syntax Extension):  JSX is a combination of HTML and JavaScript. You can embed JavaScript objects inside the HTML elements. JSX is not supported by the browsers, as a result Babel compiler transcompile the code into JavaScript code. JSX makes codes easy and understandable. It is easy to learn if you know HTML and JavaScript.

>const name="GeekforGeeks";
const ele = <h3>Welcome to {name}</h3>;

# What do you understand by Virtual DOM? Explain its working.

The Virtual DOM (VDOM) is an in-memory representation of Real DOM. The representation of a UI is kept in memory and synced with the "real" DOM. It's a step that happens between the render function being called and the displaying of elements on the screen. This entire process is called reconciliation.

In React, for every DOM object, there is a corresponding “virtual DOM object.” A virtual DOM object is a representation of a DOM object, like a lightweight copy.

A virtual DOM object has the same properties as a real DOM object, but it lacks the real thing’s power to directly change what’s on the screen.

>React uses Virtual DOM exists which is like a lightweight copy of the actual DOM(a virtual representation of the DOM. 

>So for every object that exists in the original DOM, there is an object for that in React Virtual DOM. It is exactly the same, but it does not have the power to directly change the layout of the document.

>Manipulating DOM is slow, but manipulating
Virtual DOM is fast as nothing gets drawn on the screen. So each time there is a change in the state of our application, virtual DOM gets updated first
instead of the real DOM.

 >How Virtual DOM actually make the things faster: When anything new is added to the application, a virtual DOM is created and it is represented as a tree. Each element in the application is a node in this tree. So, whenever there is a change in state of any element, a new Virtual DOM tree is created. This new Virtual DOM tree is then compared with the previous Virtual DOM tree and make a note of the changes. After this, it finds the best possible ways to make these changes to the real DOM. Now only the updated elements will get rendered on the page again.


# Why can’t browsers read JSX?

Browsers can't read JSX because there is no inherent implementation for the browser engines to read and understand them. JSX is not intended to be implemented by the engines or browsers, it is intended to be used by various transpilers to transform these JSX into valid JavaScript code. 

The browser does not understand this JSX because it's not valid JavaScript code. This is because we're assigning an HTML tag to a variable that is not a string but just HTML code.

So to convert it to browser understandable JavaScript code, we use a tool like Babel which is a JavaScript compiler/transpiler.

# What is the purpose of render() in React.

render() function takes two arguments, HTML code and an HTML element. The purpose of the function is to display the specified HTML code inside the specified HTML element.

In react, render is a method that tell react what to display. return in a method or function is the output of the method or function.

# Differentiate between states and props.

Both props and state are plain JavaScript objects. While both of them hold
information that influences the output of render, they are different in their
functionality with respect to component. Props get passed to the component
similar to function parameters whereas state is managed within the component
similar to variables declared within a function.

The key difference between props and state is that state is internal and controlled by
the component itself while props are external and controlled by whatever renders the
component

State:
State of a component is an object that holds some information that may change
over the lifetime of the component. We should always try to make our state as
simple as possible and minimize the number of stateful components.

Props:
Props are inputs to components. They are single values or objects containing a
set of values that are passed to components on creation using a naming
convention similar to HTML-tag attributes. They are data passed down from a
parent component to a child component.

# Lifecycle methods

Mounting: The component is ready to mount in the browser DOM. This phase covers initialization from constructor(), getDerivedStateFromProps(), render(), and componentDidMount() lifecycle methods.

Updating: In this phase, the component gets updated in two ways, sending the new props and updating the state either from setState() or forceUpdate(). This phase covers getDerivedStateFromProps(), shouldComponentUpdate(), render(), getSnapshotBeforeUpdate() and componentDidUpdate() lifecycle methods.

Unmounting: In this last phase, the component is not needed and gets unmounted from the browser DOM. This phase includes componentWillUnmount() lifecycle method.

# Differentiate between stateful and stateless components.

The literal difference is that one has state, and the other doesn’t. That means the stateful components are keeping track of changing data, while stateless components print out what is given to them via props, or they always render the same thing.

# How do you conditionally render components?

Conditional rendering in React works the same way conditions work in JavaScript. Use JavaScript operators like if or the conditional operator to create elements representing the current state, and let React update the UI to match them.

