# let, var, const

var: 
	- hoisted (always declared at top of scope, global if none)
    - function scope
let:
    - block scope
    - not redeclarable
const: 
    - block scope
    - not reassignable
    - not redeclarable


# value and reference type

- value => stack

- reference => heap



# heap vs stack

- 
# Prototype and prototypical inheritance

- Prototype inheritance in javascript is the linking of prototypes of a parent object to a child object to share and utilize the properties of a parent class using a child class. Prototypes are hidden objects that are used to share the properties and methods of a parent class to child classes.

# virtual dom

- React creates a virtual DOM. When state changes in a component it firstly runs a "diffing" algorithm, which identifies what has changed in the virtual DOM.

- The virtual DOM (VDOM) is a programming concept where an ideal, or “virtual”, representation of a UI is kept in memory and synced with the “real” DOM by a library such as ReactDOM. This process is called reconciliation.


# Unidirectional data flow or data binding

- Unidirectional data flow describes a one-way data flow where the data can move in only one pathway when being transferred between different parts of the program. React, a Javascript library, uses unidirectional data flow. The data from the parent is known as props.

# Event loop



# Closure



# Hydration 

- In web development, hydration or rehydration is a technique in 
which client-side JavaScript converts a static HTML web page, 
delivered either through static hosting or server-side rendering, 
into a dynamic web page by attaching event handlers to the HTML elements. 

# Hooks

- helps to control state and lifecycle without using class

- useRef - 

- useRef vs useState - If we tried to count how many times our application renders using the useState Hook, we would be caught in an infinite loop since this Hook itself causes a re-render.

# function vs method

- function - set of instruction to perform a specific task
- method - when function is inside a object its method

# Reusable hooks

# Controlled vs uncontrolled components

# HOC

A higher-order component is a function that takes in a component and returns a new component.

# What is Lifting State Up in ReactJS?

When several components need to share the same changing data then it is recommended to lift the
shared state up to their closest common ancestor. For example, if two child components share the
same data from their parent then move the state to the parent instead of maintaining the local state
in both child components.

# Why we should not update the state directly?

If you try to update state directly then it won’t re-render the component.

# When shall we use useReducer hook in ReactJS?

useReducer is an alternative to useState. useReducer is usually preferable to useState when you have
complex state logic that involves multiple sub-values or when the next state depends on the
previous one.

# Redux 

- There is a central store that holds the entire state of the application. Each component can access the stored state without having to send down props from one component to another. 

- There are three core components in Redux — actions, store, and reducers. 

- In Redux, a reducer is a pure function that takes an action and the previous state of the application and returns the new state.

# Middleware

- Middleware allows for side effects to be run without blocking state updates. We can run side effects (like API requests) in response to a specific action, or in response to every action that is dispatched (like logging). 


# Pure functions 

- Pure functions return the same output if we use the same input parameters. However, impure functions give different outcomes when we pass the same arguments multiple times

# Optimization

lighthouse




# Testing



# Why we should not update the state directly?

The state of a component is managed internally by React. Updating the state of a component directly can have unintended consequences that can be difficult to debug. If the state is updated directly as in the example above, the component will not rerender since the state is compared shallowly.