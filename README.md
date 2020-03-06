Tutorial App

npx create-react-app
npm i react-router-dom
npm i axios

FEATURES 

Fetching data from an API using axios,
Using Context API for state management and storing global states

CONTEXT 

Create a context.js file in root
Uses the const Context = React.createContext(); hook.
Create a Provider class functions which will store global function and states
and render as Context.Provider , all components which are to use the states needs to be wrapped
within Provider tag.
export as export const Consumer = Context.Consumer; so the Provider will store the states while
the Consumer delivers them to the app

DIFFERENCE BETWEEN FUNCTION AND CLASS BASED COMPONENTS

Function based components also called as stateless components are used when the component doesnt require
or holds any state of its own and will not use any of the lifecycle hooks. Stateless components are preffered
and should used whenever possible.

Class based componenets also can use lifecycle hooks such as ComponentDidMount() or Constructor() and can be
used in cases such as fetching an api which requires to run after the page is rendered.

AXIOS

axios.get('api.url')
.then( res => {})
.catch( err => {})

MAP

ES6 map method is used to copy an array and loop for the items it contains and render then in a component
Looped components require a key value and prop value so that it can recognize the value its being passed on.
In the component that you are using the map function on you need to pass the props as an argument at initial function

itemsArray.map( item => (
    Component key={item.id} item={item}
))