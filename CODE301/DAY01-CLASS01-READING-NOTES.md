# CODE FELLOWS - CODE 301

## DAY 01 CLASS 01

### [HOME](../README.md)

## AGENDA
1. React and Component-Based Architecture
1. Initialize React Application

## READING
[Component-Based Architecture](https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm)

[What is Props and How to Use it in React](https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0)

## ADDITIONAL RESOURCES

## READING NOTES
### Component-Based Architecture
1. What is a “component”?
    * "A component is a modular, portable, replaceable, and reusable set of well-defined functionality that encapsulates its implementation and exporting it as a higher-level interface."

    * "A component is a software object, intended to interact with other components, encapsulating certain functionality or a set of functionalities. It has an obviously defined interface and conforms to a recommended behavior common to all components within an architecture."

    * "A software component can be defined as a unit of composition with a contractually specified interface and explicit context dependencies only. That is, a software component can be deployed independently and is subject to composition by third parties."

1. What are the characteristics of a component?
    * "Reusability − Components are usually designed to be reused in different situations in different applications. However, some components may be designed for a specific task."

    * "Replaceable − Components may be freely substituted with other similar components."

    * "Not context specific − Components are designed to operate in different environments and contexts."

    * "Extensible − A component can be extended from existing components to provide new behavior."

    * "Encapsulated − A A component depicts the interfaces, which allow the caller to use its functionality, and do not expose details of the internal processes or any internal variables or state."

    * "Independent − Components are designed to have minimal dependencies on other components."

1. What are the advantages of using component-based architecture?
    * "Ease of deployment − As new compatible versions become available, it is easier to replace existing versions with no impact on the other components or the system as a whole."

    * "Reduced cost − The use of third-party components allows you to spread the cost of development and maintenance."

    * "Ease of development − Components implement well-known interfaces to provide defined functionality, allowing development without impacting other parts of the system."

    * "Reusable − The use of reusable components means that they can be used to spread the development and maintenance cost across several applications or systems."

    * "Modification of technical complexity − A component modifies the complexity through the use of a component container and its services."

    * "Reliability − The overall system reliability increases since the reliability of each individual component enhances the reliability of the whole system via reuse."

    * "System maintenance and evolution − Easy to change and update the implementation without affecting the rest of the system."

    * "Independent − Independency and flexible connectivity of components. Independent development of components by different group in parallel. Productivity for the software development and future software development."

### What is “Props” and how to use it in React?
1. What is “props” short for?
    * "Props is a special keyword in React, which stands for properties and is being used for passing data from one component to another."

1. How are props used in React?
    1. Firstly, define an attribute and its value(data)
    2. Then pass it to child component(s) by using Props
    3. Finally, render the Props Data

1. What is the flow of props?
    * "Props can only be passed to components in one way (parent to child)"

## CLASS NOTES

### OLD WAY OF MAKING CONSTRUCTORS

```js
functions Musician(artist, style) {
	this.artist = artist;
	this.style = style;
	this.isAmazing = true;
}

let edSheeran = newMusician('Ed Sheeran', 'indy');
```
### NEW WAY OF MAKING CLASSES

```js
class MusicianClass {
	constructor(artist, style){
	this.artist = artist;
	this.style = style;
	}
	awesome = () => {console.log('awesome!');}
```

### ARROW FUNCTIONS
    Arrow functions inherit the scope from where they are declared (inherit the context)

    Arrow functions are very useful when dealing with classes

## LINKS
* [Class 01 GitHub](https://github.com/codefellows/seattle-code-301d85/tree/main/class-01)

* [React Tutorial through ‘Passing Data Through Props’](https://reactjs.org/tutorial/tutorial.html)
* [React Docs - Hello world](https://reactjs.org/docs/hello-world.html
)
* [React Docs - Introducing JSX](https://reactjs.org/docs/introducing-jsx.html)
* [React Docs - Rendering elements](https://reactjs.org/docs/rendering-elements.html)
* [React Docs - Components and props](https://reactjs.org/docs/components-and-props.html)

## VOCABULARY

## THINGS I WANT TO KNOW MORE ABOUT

## LEARNING THAT OCCURRED AND PROBLEMS THAT ARE SOLVED

Today I learned that I can write the language after \`\`\` to get Markdown to format automatically and add colors.  Like \`\`\`js or \`\`\`html.

## PROBLEMS THAT HAVE TIMED OUT BEFORE RESOLUTION

### [HOME](../README.md)