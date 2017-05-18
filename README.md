### Usage Instructions

#### To run the app,
1. Make sure `mongodb` is running in the background. 
2. Install global dependencies with `npm install -g gulp bower react-tools browserify`
3. Install dependencies with `npm install; bower install`
4. Run app with `gulp serve`


### Glossary

## Dispatcher
A simple emitter. Object register with the emitter to listen for an event, and when the event occurs, the objects are notified.

## Store
A utility that listens for particular kind of dispatcher events and is responsible for the handling of one element.

## State
A React component's state. A component can change it's own state, but not the state of other components. In order to change the state of another component, an app must make the appropriate request to a store.

## Props
The properties of a React component. A component cannot change its own properties. The properties of a React component can only be set by its parent. In order to change the props of a component which is not the child of the caller, a request must be passed to the appropriate store.

## JSX
A React-specific variant of JavaScript. JSX can be compiled into JavaScript code containing React components. JSX must be compiled as it cannot be read by web browsers. 

### JSX Transformer
A tool used to transform JSX without any backend. Can be used in the browser. Not used for production.

### Reactify
A useful Browserify plugin which compiles JSX in to JavaScript as it is being browserified.