# CODE FELLOWS - CODE 301

## DAY 03 CLASS 03

### [HOME](../README.md)

## AGENDA
1. Functions as Props
1. Manipulate state from child component via passed function

## READING

* [React Docs - lists and keys](https://reactjs.org/docs/lists-and-keys.html)
* [Coding at Dawn - The Spread Operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)
* [Steven Griffith - How to Pass Functions between Components](https://www.youtube.com/watch?v=c05OL7XbwXU)

## ADDITIONAL RESOURCES

* [React - Tutorial](https://reactjs.org/tutorial/tutorial.html)
* [React - Lifting State Up](https://reactjs.org/docs/lifting-state-up.html)

## READING NOTES

### What does .map() return?
* It appears to return all items in an array.

### If I want to loop through an array and display each value in JSX, how do I do that in React?
* ```console.log(array.map(value))```

### Each list item needs a unique ```key```.

### What is the purpose of a key?
* "Keys help React identify which items have changed, are added, or are removed."

### What is the spread operator?  
* The use of ellipsis ```...``` to expand objects

### List 4 things that the spread operator can do.
1.  adding items to arrays
1.  combining arrays
1.  combining objects
1.  spreading an array out into a function's arguments

### Give an example of using the spread operator to combine two arrays.
* ```let newArray = [...array1,...array2];```

### Give an example of using the spread operator to add a new item to an array.
* ```let newArray = [newValue1, newValue2,...oldArray];```
* Other coding examples in the article still used ```array.pop()```

### Give an example of using the spread operator to combine two objects into one.
* ```let newObject = {...object1,...object2};```

### In the video, what is the first step that the developer does to pass functions between components?

### In your own words, what does the increment function do?

### How can you pass a method from a parent component into a child component?

### How does the child component invoke a method that was passed to it from a parent component?

## CLASS NOTES

## LINKS
### [Class 03 GitHub](https://github.com/codefellows/seattle-code-301d85/tree/main/class-03)

## VOCABULARY

## THINGS I WANT TO KNOW MORE ABOUT

## LEARNING THAT OCCURRED AND PROBLEMS THAT ARE SOLVED

## PROBLEMS THAT HAVE TIMED OUT BEFORE RESOLUTION

### [HOME](../README.md)