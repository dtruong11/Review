1. What does HTML stand for?

<details>
  <summary>Answer here</summary>
  Hypertext Markup Language
</details>

2. Define React component?

<details>
  <summary>Answer here</summary>
  A chunk of a website that can be reused - includes JS, CSS, HTML
</details>

3. Describe the different types of React Component?

<details>
  <summary>Answer here</summary>
  1. Function component:  a function that returns a single React Element.
  2. Class component: A JavaScript class that extends React.Component; must have a render method. 
</details>

4. Describe the differences between class and function component (also in relation to props)?

<details>
  <summary>Answer here</summary>
  1. Function component:  stateless; use destructuring to access props.
  2. Class component: saves state; must use this.props.object after using the super keyword; must have a render method. 
</details>

5. What do you use to pass data into components? Define that?

<details>
  <summary>Answer here</summary>
    Props: an object passed from parent to child. 
</details>

6. What is controlled component?

<details>
  <summary>Answer here</summary>
  Controlled component: manages its own state. Form can be constructed as a controlled component. 
</details>

7. Describe the error of directly managing state? 

<details>
  <summary>Answer here</summary>
  this.state = something 
</details>

8. Define state? What are some examples of where we've managed state thus far?

<details>
  <summary>Answer here</summary>
  State is the data structure, and view reflects it within the DOM. Login/Logout would change the state of multiple elements.
</details>

9. What keyword should you use to change state in React? 

<details>
  <summary>Answer here</summary>
  this.setState({ data : newData })
</details>

10. Define React lifecyle?

<details>
  <summary>Answer here</summary>
  The life of a React component, from birth (pre-mounting) and death (unmounting).
  Through lifecycle methods, we can then control what happens when each tiny section of your UI renders, updates, thinks about re-rendering, and then disappears entirely.
</details>