# CODE FELLOWS - CODE 301

## DAY 02 CLASS 02

### [HOME](../README.md)

## AGENDA
1. React State and Props
1. Create gallery of images from common state

## READING
1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?
    * The rendering happens first.

1. What is the very first thing to happen in the lifecycle of React?
    * Mounting.

1. Put the following things in the order that they happen: 
    1. constructor
    1. render
    1. React Updates
    1. componentDidMount
    1. componentWillUnmount

1. What does componentDidMount do?
    * It is used for load thing using a network request or initializing the DOM.

## VIDEOS
1. What types of things can you pass in the props?
    * Data for rendering
    * Information

1. What is the big difference between props and state?
    * Props get handled outside the component and are passed in.  State is handled inside the component.

1. When do we re-render our application?
    * A component will re-render an application when state is changed.

1. What are some examples of things that we could store in state?
    * Dynamic items

## ADDITIONAL RESOURCES

## READING NOTES
React components are classes or functions.  We'll be using classes in 301 and functions in 401.

Methods that can be used are called lifecycle events.

Mounting, Updating, and Unmounting are the three phases of the component lifecycle.

Avoid using this.setState() in the constructor because it can lead to side effects, and it is unnecessary. Doing this will ignore all updates to props, so it shouldn’t be done unless it is intentional.

Render is the only required method in a class component.

Props are like arguments (parameters) to a function.

If information is going to change or only going to exist inside a component it should be state.

If information is static or gets provided or shared between components it should be a prop.

State is similar to props, but it is private and fully controlled by the component.

## CLASS NOTES

## LINKS
### [Class 02 GitHub](https://github.com/codefellows/seattle-code-301d85/tree/main/class-02)
### [React Lifecycle](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)
### [React State vs Props](https://www.youtube.com/watch?v=IYvD9oBCuJI)

### [React Docs - State and Lifecycle](https://reactjs.org/docs/state-and-lifecycle.html)
### [React Docs - handling events](https://reactjs.org/docs/handling-events.html)
### [React Tutorial through ‘Developer Tools’](https://reactjs.org/tutorial/tutorial.html)
### [React Bootstrap Documentation](https://react-bootstrap.github.io/)
### [Boootstrap Cheatsheet](https://getbootstrap.com/docs/5.0/examples/cheatsheet/)
### [Bootstrap Shuffle - a class “sandbox”](https://bootstrapshuffle.com/classes)
### [Netlify](https://www.netlify.com/)

## VOCABULARY

## THINGS I WANT TO KNOW MORE ABOUT

Converting a Function to a Class
You can convert a function component like Clock to a class in five steps:

1. Create an ES6 class, with the same name, that extends React.Component.
1. Add a single empty method to it called render().
1. Move the body of the function into the render() method.
1. Replace props with this.props in the render() body.
1. Delete the remaining empty function declaration.

FUNCTION
```js
const root = ReactDOM.createRoot(document.getElementById('root'));
  
function tick() {
  const element = (
    <div>
      <h1>Hello, world!</h1>
      <h2>It is {new Date().toLocaleTimeString()}.</h2>
    </div>
  );
  root.render(element);
}

setInterval(tick, 1000);
```

CLASS
```js
class Clock extends React.Component {
  constructor(props) {
    super(props);
    this.state = {date: new Date()};
  }

  componentDidMount() {
    this.timerID = setInterval(
      () => this.tick(),
      1000
    );
  }

  componentWillUnmount() {
    clearInterval(this.timerID);
  }

  tick() {
    this.setState({
      date: new Date()
    });
  }

  render() {
    return (
      <div>
        <h1>Hello, world!</h1>
        <h2>It is {this.state.date.toLocaleTimeString()}.</h2>
      </div>
    );
  }
}

const root = ReactDOM.createRoot(document.getElementById('root'));
root.render(<Clock />);
```

## LEARNING THAT OCCURRED AND PROBLEMS THAT ARE SOLVED

## PROBLEMS THAT HAVE TIMED OUT BEFORE RESOLUTION

### [HOME](../README.md)