# Class-Based Components
***An Alternative Way Of Building Components***

- What & Why?
- Working with Class-based Components
- Error Boundaries
---
**Class Components vs. Functional Components**

**Functional Components:** Components are regular JavaScript function which return renderable results (typically JSX)

** The default & most modern approach!

`function Product(props) {`

`return <h2>A Product!</h2>`

`}`

**Class-based Components:** Components can also be defined as JS classes where a render() method defines the to-be rendered output

** Was required in the past

`class Product extends Component {`

`render() {`

`return <h2>A Product!</h2>`

`}`

`}`
---
**When using React prior to version 16.8;**

Traditionally, you had to use class-based components to manage ***“State”***

React 16.8 introduced ***“React Hooks”*** for ***functional*** components

***Class-based*** components ***can’t use*** React Hooks

---

['this' Keyword & Function References][def]


[def]: https://academind.com/tutorials/this-keyword-function-references/

---
**Class Components Lifecycle**

***Side Effects*** in ***Functional*** Components: **useEffect() ⇒ *Class-based*** components ***can’t use*** React Hooks

**ComponentDidMount()** : Called once a component ***mounted*** / evaluated & rendered by React ⇒ `useEffect(…, [])`

**ComponentDidUpdate()** : Called once a component ***updated*** / re-evaluated & re-rendered by React ⇒ `useEffect(…, [someValue])`

**ComponentWillUnmount()** : Called right before component is ***unmounted*** / right before removed from DOM ⇒ `useEffect(() ⇒ { return () ⇒ {…} }, [])`
