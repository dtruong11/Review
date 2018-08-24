## Define pure functions?

<details>
    <summary>Answer here</summary>
     1. A pure function doesn’t depend on and doesn’t modify the states of variables out of its scope.
     2. a pure function always returns the same result given same parameters. 
</details>

## Define Provider (a redux concept)? 

<details>
    <summary>Answer here</summary>
 	
    ```javascript
        import React from 'react';
        import ReactDOM from 'react-dom';
        import App from './components/App';
        import { Provider } from 'react-redux'
        import store from './store'
        import '../node_modules/bootstrap/dist/css/bootstrap.min.css'
        import registerServiceWorker from './registerServiceWorker'


        ReactDOM.render(
        <Provider store={store()}>
            <App />
        </Provider>,
        document.getElementById('root')
        );
        registerServiceWorker()
    ```
    make the store available to all container components in the application without passing it explicitly. You only need to use it 	once when you render the root component:
</details>



## When do we need to use dispatch() (redux concept)?

<details>
    <summary>Answer here</summary>
    Dispatch is a function that is used for sending actions. 
    It accepts a function as its argument. 
    Action creators often trigger a dispatch when invoked. 
    
    ```  
        function addTodoWithDispatch(text) {
        const action = {
            type: ADD_TODO,
            text
        }
        dispatch(action)
        }
    ```

</details>


## Define reducers? 

<details>
    <summary>Answer here</summary>
    Reducers are just pure functions that take the previous state and an action, and return the next state. Remember to return new state objects, instead of mutating the previous state.
</details>


## Define store (Redux)

<details>
    <summary>Answer here</summary>
    The state of your whole application is stored in an object tree within a single store. It's just an object with a few methods on it.
    To create it, pass your root reducing function to createStore.
	* easier to debug
    * Easier to create universal apps 

</details>


## Define mapStateToProps

<details>
    <summary>Answer here</summary>
    If you want to establish some initial state on our components, you can pass values as props into a function called mapStateToProps and then pass it as the first parameter to connect.
</details>


## Define MapDispatchToProps

<details>
    <summary>Answer here</summary>
    The connect method can also take a second argument that is a function that adds the action creators to the propsobject. In the case that all you need are your action creators, but not your access to your store state, you can replace mapStateToProps with null. 

</details>


## React Router Review

## Define Switch/Route

<details>
    <summary>Answer here</summary>
     1. <Switch> Renders the first child <Route> or <Redirect> that matches the location.
     2. <Switch> is unique in that it renders a route exclusively. In contrast, every <Route> that matches the location renders inclusively.
</details>

## What do you import from react-router-dom to wrap around your components in the index?

<details>
    <summary>Answer here</summary>
     BrowserRouter
</details>


## Which keyword do you use to match a specific path or URL?

<details>
    <summary>Answer here</summary>
     Exact.
</details>

## Name the two ways to render components

<details>
    <summary>Answer here</summary>
     1. Render Component - A React component to render only when the location matches.
     2. Render Function - This allows for convenient inline rendering and wrapping without the undesired remounting explained above.
</details>

## Name the two ways to render components

<details>
    <summary>Answer here</summary>
     1. Render Component - A React component to render only when the location matches.
     2. Render Function - This allows for convenient inline rendering and wrapping without the undesired remounting explained above.
</details>

## What is Redux Thunk?

<details>
    <summary>Answer here</summary>
    Redux Thunk middleware allows you to write action creators that return a function instead of an action. The thunk can be used to delay the dispatch of an action, or to dispatch only if a certain condition is met. The inner function receives the store methods dispatch and getState as parameters.
</details>

## What higher-order component do you use to get access to the history object's properties and the closest <Route>'s match?

<details>
    <summary>Answer here</summary>
    withRouter
</details>


