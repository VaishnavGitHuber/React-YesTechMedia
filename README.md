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

### MODULE 3: Components 
- **Components** (one of many pieces) are used to break the complex UI structures into small managable pieces, can be achieved in 2 ways,
  1. Function Components
  2. Class Components
- **rafce** keyboard short cut to create components faster.
- Create a folder inside **src** folder named components, create Components inside the folder.

---


