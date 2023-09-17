

https://github.com/sakmaruvijay/calc-react-redux
# Counter App with Redux 

Basic React App showcasing how Redux works and connects with React.JS



## Live Demo
https://sakmaruvijay.github.io/calc-react-redux-page


## Getting Started
Below instructions will get you a copy of the project. You can run on your local machine for development and testing purposes.



### Installing

```
git clone  https://github.com/sakmaruvijay/calc-react-redux
```

```
npm install
```

```
npm run
```







## Dependencies 

    "react": "^16.3.2",
    "react-dom": "^16.3.2",
    "react-redux": "^5.0.7",
    "react-scripts": "1.1.4",
    "redux": "^4.0.0"



  ##  Basic Flow 
Now, let's see how the data flow works:

Components trigger actions: When a user interacts with a component, such as clicking a button, the component triggers an action. An action is a plain JavaScript object that describes the intention to change the state. It typically has a type property to indicate the type of action being performed and may include additional data.

Actions are dispatched to the store: The component dispatches the action to the Redux store using the dispatch function. The store receives the action and forwards it to the reducers.

Reducers update the state: Each reducer receives the action and the current state that it is responsible for. Based on the action type, the reducer creates and returns a new state object that reflects the changes triggered by the action. The new state is then stored in the store.

Store notifies connected components: Once the state is updated, the store notifies the connected components (containers) that subscribed to the relevant parts of the state. The containers receive the updated state as props and pass it down to the child components.

Components re-render with new data: When a connected component receives new props (updated state), it re-renders with the new data. The updated UI is displayed to the user, reflecting the changes in the application's state.

This data flow ensures that the state is managed centrally in the store, actions are dispatched to modify the state, reducers update the state immutably, and the updated state is propagated to the relevant components for re-rendering.

By following this pattern, React with Redux provides a predictable and efficient way to manage the state of your application, making it easier to maintain and scale as the application grows.





