# CODE FELLOWS - CODE 301

## DAY 05 CLASS 05

### [HOME](../README.md)

## AGENDA
1. 	Conditional Rendering, Routing
1. 	Portfolio - 3rd party application modifications

## READING
### React Docs - Thinking in React
1. What is the single responsibility principle and how does it apply to components?

    * "SRP is a computer-programming principle that states that every module, class or function in a computer program should have responsibility over a single part of that program's functionality, and it should encapsulate that part." -[wikipedia](https://en.wikipedia.org/wiki/Single-responsibility_principle)
    * A component should ideally only do one thing.  If it ends up growing, it should be decomposed into smaller sub-components.

1. What does it mean to build a ‘static’ version of your application?
    * Building a version that takes a data model and renders the UI but has no interactivity.

1. Once you have a static application, what do you need to add?
    * interactivity 

1. What are the three questions you can ask to determine if something is state?
    1. Is it passed in from a parent via props? If so, it probably isn’t state.
    1. Does it remain unchanged over time? If so, it probably isn’t state.
    1. Can you compute it based on any other state or props in your component? If so, it isn’t state.

1. How can you identify where state needs to live?
    * For each piece of state in your application:
      1. Identify every component that renders something based on that state.
      1. Find a common owner component (a single component above all the components that need the state in the hierarchy).
      1. Either the common owner or another component higher up in the hierarchy should own the state.
      1. If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.



### Higher-Order Functions
1. What is a “higher-order function”?
    * "Functions that operate on other functions, either by taking them as arguments or by returning them."

1. Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?
    * It is returning m if m is greater than n.

1. Explain how either map or reduce operates, with regards to higher-order functions.
    * "The map method transforms an array by applying a function to all of its elements and building a new array from the returned values. The new array will have the same length as the input array, but its content will have been mapped to a new form by the function."
    * "[Reduce] builds a value by repeatedly taking a single element from the array and combining it with the current value."

## ADDITIONAL RESOURCES

## READING NOTES
### BUILDING APPS
To build a static version of your app that renders your data model, you’ll want to build components that reuse other components and pass data using props. props are a way of passing data from parent to child. If you’re familiar with the concept of state, don’t use state at all to build this static version. State is reserved only for interactivity, that is, data that changes over time. Since this is a static version of the app, you don’t need it.

When building simpler projects, it’s usually easier to go top-down, and on larger projects, it’s easier to go bottom-up and write tests as you build.

### GREATER THAN
```js
function greaterThan(n) {
  return m => m > n;
}
let greaterThan10 = greaterThan(10);
console.log(greaterThan10(11));
// → true
```
### MAP
The map method transforms an array by applying a function to all of its elements and building a new array from the returned values. The new array will have the same length as the input array, but its content will have been mapped to a new form by the function.

```js
function map(array, transform) {
  let mapped = [];
  for (let element of array) {
    mapped.push(transform(element));
  }
  return mapped;
}

let rtlScripts = SCRIPTS.filter(s => s.direction == "rtl");
console.log(map(rtlScripts, s => s.name));
// → ["Adlam", "Arabic", "Imperial Aramaic", …]
```
### REDUCE
The parameters to reduce are, apart from the array, a combining function and a start value. This function is a little less straightforward than filter and map, so take a close look at it:

```js
function reduce(array, combine, start) {
  let current = start;
  for (let element of array) {
    current = combine(current, element);
  }
  return current;
}

console.log(reduce([1, 2, 3, 4], (a, b) => a + b, 0));
// → 10
```

The standard array method reduce, which of course corresponds to this function, has an added convenience. If your array contains at least one element, you are allowed to leave off the start argument. The method will take the first element of the array as its start value and start reducing at the second element.

```js
console.log([1, 2, 3, 4].reduce((a, b) => a + b));
// → 10
```

## CLASS NOTES

## LINKS
### [Class 05 GitHub](https://github.com/codefellows/seattle-code-301d85/tree/main/class-05)
### [React Docs - Thinking in React](https://reactjs.org/docs/thinking-in-react.html)
### [Higher-Order Functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)

## VOCABULARY

## THINGS I WANT TO KNOW MORE ABOUT

## LEARNING THAT OCCURRED AND PROBLEMS THAT ARE SOLVED

## PROBLEMS THAT HAVE TIMED OUT BEFORE RESOLUTION

### [HOME](../README.md)