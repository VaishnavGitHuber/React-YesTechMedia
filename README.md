## React Fundamantals 

---

#### MODULE 1 : Introduction & Installation 
- React is a frontend framework devoloped by facebook in 2013.
- React follows component based architechture.
- It uses virtual DOM.

---

#### MODULE 2 : JSX(Javascript syntax Extension / Javascript XML) 
- Javascript syntax Extension(JSX) allows to combine HTML & JS in a single file.
- **Babel** compiles the Javascript in the JSX.(working of JSX)
- **JSX Attributes:** JSX attributes are similar to HTML syntax with some slight differences.(provide extra information about the element)
  ```
  <h1 class='heading'>This is heading</h1> // html attribute
  <h1 className = 'heading'>This is a heading</h1> //JSX syntax
  ```
  here, JSX uses camelcase for the attributes unlike HTML(lowercase).
- **JSX Expressions:** JSX allows to embed JS expressions in Html,it uses curly braces {} to achieve this.
  ```
  function Welcome(){
    return (
      <div>
        let name = "krishna"
        <h1>My name is: {name}</h1> // embedding variable expression
        <h2>Sum of 4 & 5 :{4 + 5}</h2> // expression
      </div>
    )
  }
  ```
- **JSX Fragment** JSX Fragments are used to group multiple elements without adding an extra node.
  ```
  function Welcome(){
    return (
      <> // JSX Fragment 
        let name = "krishna"
        <h1>My name is: {name}</h1> // embedding variable expression
        <h2>Sum of 4 & 5 :{4 + 5}</h2> // expression
      </>
    )
  }
  ```
  also, we can use <React.Fragment></React.Fragment> to achieve this.

---

#### MODULE 3 : Components 
- **Components** (one of many pieces) are used to break the complex UI structures into small managable pieces, can be achieved in 2 ways,
  1. Function Components
  2. Class Components
- **rafce** keyboard short cut to create components faster.
- Create a folder inside **src** folder named components, create Components inside the folder.

---
#### MODULE 4 : CSS in react
- There are 3 ways of adding css in react,
  1. Inline css
     ```
     <h1 style={{color='red'}}>This is heading</h1>
     ```
  2. using variable
     ```
     const styleHeading = {color='red'};
     <h1 style={styleHeading}>This is heading</h1>
     ```
  3. Using external CSS file
     ```
     import "./App.css" // external css file App.css
     <h1 className='heading'>This is heading</h1>
     ```
---

#### MODULE 5 : Bootstrap in react
1. step 1 : install bootstrap using npm
```
npm install react-bootstrap bootstrap
```
2. step 2 : import bootstrap in App.js or index.js
```
import "bootstrap/dist/css/bootstrap.min.css"
```
3. step 3 : import required classes
```
import {Button, Navbar} from 'react-bootstrap'
```
#### MODULE 6 : Events in react 
- **Events** are the user actions over the web pages.
- Events are written as camel case(eg: onClick)
- examples(onClick, onDoubleClick, onChange, onKeyDown, onMouseOver)
```
const clickHandle = () => {
  alert("You click the mouse")
  }
<button onClick = {clickHandle} >Click Me</button>
```
#### MODULE 7 : useState & Hook function
- **state** : state is a object that stores **value of the properties of the components** that could change.
- evert time when state changes, react rerender the component to the browser.
- **Hook Function** : Hook functions are the special functions that let's you to hook into react features.
- **useState** is a hook function that **allow to add state to the component**, modify the state of the component.
```
import {useState} from 'react'

const [count, setCount] = useState(0) // count - set the current state value, setCount - function to update the state
```
#### MODULE 8 : Props(properties) in react 
- props are the **arguments passed to the react components.**
- It is similar to the function arguments.
```
function App(props){
  return (
    <h1>Name: {props.name}</h1>
    )
}

<App name={"Vaishnav"} />
```
