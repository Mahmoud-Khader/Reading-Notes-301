# Read03

## React Docs - lists and keys

1-*What does .map() return?*

**return the new array**

2-*If I want to loop through an array and display each value in JSX, how do I do that in React?*

**You can build collections of elements and include them in JSX using curly braces {} and render it to the DOM**

3-*Each list item needs a unique ____.*

**KEY**

4-*What is the purpose of a key?*

**a special string attribute you need to include when creating lists of elements**


## The Spread Operator

1-*What is the spread operator?*

**is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.**

2-*List 4 things that the spread operator can do.*

* Copying an array
* Concatenating or combining arrays
* Adding an item to a list
* Adding to state in React

3-*Give an example of using the spread operator to combine two arrays.*

>const myArray = [`1`,`2`,`3`]
const yourArray = [`4`,`5`,`6`]
const ourArray = [...myArray,...yourArray]
console.log(...ourArray) // 1 2 3 4 5 6

4-*Give an example of using the spread operator to add a new item to an array.*

> const myArray = ['1','2','3']
const moreArray = ['4', '5', ...moreNumbers]
console.log(moreArray) //  Array(5) [ "4", "5", "1", "2", "3" ]

5-*Give an example of using the spread operator to combine two objects into one.*

> const objectOne = {hello: "🤪"}
const objectTwo = {world: "🐻"}
const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
objectFour.laugh() // 😂😂😂😂😂 


## How to Pass Functions Between Components

1-In the video, what is the first step that the developer does to pass functions between components?

**create a function wherever the state is that we are going to change.**

2-In your own words, what does the increment function do?

**is recive an object , and loop inside the array using map method , then find the matching name and update the count by one**

3-How can you pass a method from a parent component into a child component?

**by using constructor keyword then spicify the methods using supr() method.**

4-How does the child component invoke a method that was passed to it from a parent component?

**by using the state method , it can from them invoke the method and update the component methods or attreputs.**