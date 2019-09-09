{% include "../includes/header.md" %}

# Prep Work - Objects and Arrays

*“Another flaw in the human character is that everybody wants to build and nobody wants to do maintenance.” - Kurt Vonnegut*

## Purpose

<!-- Here is where we will tell the students the "WHY" behind what they're about to read and learn about. Then we'll give them an overview of the material, sort of a "Big Picture" of the new concept so they can go in with a context of the very NEW material.  -->
So far we've been working with primitive data types, such as numbers, strings, and booleans.  These are great for storing small isolated bits of information, but what happens when you want to store related information such as the make, model, and color of all the cars in a car dealership?  Or if you want to store the names of all of a user's friends on a social media platform?  By using objects and arrays we can group related pieces of data together in a way that makes our database easier to access and manipulate.

******

<!-- ## Prep For Your Career

### Purpose - Why Is This Important? -->

<!-- This is where we give them a background to the history or common practice in the industry. We must remember they have no idea how the tech world works. Give them the why behind the ACTION ITEM -->
<!-- Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum
Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum

### Action Item -->

<!-- This is a specific task they can do. It needs to be small and make them feel they are actually contributing to the their career, LinkedIn profile update, follow people on medium, youTube, GitHub, Reddit, Hackernews, etc... -->
<!-- Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum
Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum

### Q&A - Topic

**Question: The question?** -->
<!-- Should include a short video clip of a grad asking a question about the topic. This will bring them context to the what their doing and why its important. Again, always instilling confidence!! -->
<!-- <iframe width="560" height="315" src="https://www.youtube.com/embed/XQu8TTBmGhA" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe> -->

## Arrays

An [array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array) is a specialized object in Javascript.  In other words, all arrays are objects, but not all objects are arrays.  Arrays are useful for storing items in a manner in which order is important, or for grouping lists of items together. Most of the time, when you have  a list you should consider storing your data in an array.

An array looks like this:

```javascript
['item1', 'item2', ...];
```

### Read it - Programming with Arrays

You can declare an array just like you would declare a variable.  Just put the array inside [] brackets and separate the items in an array with a comma (see below).

```javascript
const exampleArray = ['h','e','l','l','o']
const ourCarTypes = ["Saab", "Volvo", "BMW"]
const itemArray = ['item1', 'item2']
const arrayOfNumber = [1, 200, 98, 75, 4, 4000]

```

Items in an array each have an index that represents the order in which they appear. **Arrays are 0 indexed**. This means the first item in an array has an index of 0.  You access items in an array by their index. Using the example above: `console.log(exampleArray[1])` would log to the console `e` (because arrays are zero indexed to access `'h'` you would need to use exampleArrary[0]). You can re-assign items in a similar manner. `exampleArrary[1] = ‘y’` would rewrite the array to look like this: `[‘h’,’y’,’l’,’l’,’o’]`

The items stored in an array can be of any data type you learned about so far, primitive or higher order(like an object or function): Number, null, string, array, object, function, node, etc.  When we put arrays inside arrays we call this *nesting*. This means you can store an array or multiple arrays inside an array or store objects inside an array. See below:

```javascript
const multiArrays = [[1, 2, 3, 6, 9, 5], [90, 5, 8, 65, 3], ["dog", "tooth", "friend"]]

console.log(multiArrays[1]) // => [90, 5, 8, 65, 3]
console.log(multiArrays[0]) // => [1, 2, 3, 6, 9, 5]
console.log(multiArrays[2][2]) // => "friend"
```

#### Array Methods

You might not have seen the word method yet but for not simply think of them as baked-in function that Javascript comes with. You don't have to do anything special to get them to work all you have to do is learn about them and then call them by name. As you learn more about the language you'll come to learn and appreciate all of the wonderful methods Javascript has to offer.

For now, just know that arrays come with some of the most powerful methods in the Javascript environment!

As an example, `.length` is a simple and yet very powerful method use all the time! Using `.length` on an array will return the number of items in the array. Example: If we `console.log(multiArrays.length)` from above we would get `3`. If we `console.log(multiArrays[0].length)` we would get `6`. You get get it? *Hint: The index of the last item in an array is always equal to the `.length` of the array minus one. (`console.log(multiArrays[1].length - 1) // => 4`)

**Play with Array Methods**
Start looking at these [array methods](https://www.w3schools.com/Jsref/jsref_obj_array.asp) and see if you can play with some dummy variables with them. Simple copy paste some of the code snippets above into a [repl.it]()https://repl.it/repls, add more data to them and try some of these methods inside a `console.log` statement. See what you come up with

In programming, there's a word called *mutability*. This simply means that the original data can be changed or is permanently changed.  Permanently changing the original data/data structure is something that should generally be avoided. This is where the word, immutable comes. While your discovering the various array methods, make sure that you know what the *method returns* and if the method permanently changes the data of the original array on which you called it on. You'll learn when to change data and when not to as you go [deeper](https://www.codingame.com/playgrounds/6181/javascript-arrays---tips-tricks-and-examples) but for now just become aware of what each methods returns and if it's changing the original array. 

An example of a method that mutates the original array is `.push()` : `exampleArray.push(‘x’)`.  This method would add the string `'x'` to the end of `exampleArray` and thereby permanently change the array.  The push method also returns the new length of the string.  So if exArr had 5 elements, and you declared `const newLength = exampleArray.push('x')`, `newLength` would be equal to 6, and the string 'x' would be added to the end of `exampleArray`.

Adding new items to an array can also be accomplished without mutation by using the concat method, which merges two arrays, or merges values into an array: `const exArr2 = exampleArray.concat('x')`.  In this case, `exampleArray` would not be changed, and `exArr2` would be the same as `exArr`, but with the string `'x'` added to the end of the array.  This is an example of a *non-mutating* array method.

To learn more about mutating and not-mutating array methods you can check out this [blog post](https://lorenstewart.me/2017/01/22/javascript-array-methods-mutating-vs-non-mutating/), but keep in mind that unlike in this article, most cases you will want to declare all of your arrays with `const`, not `let`, whether or not you intend to mutate them.

#### Nesting Arrays

As we saw above we can nest arrays or objects within arrays. Arrays within arrays are called multidimensional arrays. The arrays inside a multidimensional array are known as nested arrays. You would access and set nested values in a similar manner to how you would access any array value. First you would access the item (the nested array), then you would access the item in that array using the return.

Let's look at an example

```javascript
const numArr = [
    [4, 7, 9],
    [10, 45, 300],
    [88, 64, 37, 93]
];
```

To access the number 300 in this array, first access the second array, then access the third item in that array. `numArr[1][2]`

*BIG NOTE: One important thing to remember about arrays: **no two arrays are the same array**. So, even if you declared:

```javascript
const arr1 = [1,2,3]
const arr2 = [1,2,3]

arr1 === arr2 // =>  false
```

**How would you find out if two arrays contain the same values?  Think about it and see if you can come up with an answer before class.**

******

#### Practice Array Methods

**Experiment with arrays and popular array methods below:**

{% tonic %}

//Create an array
const students = ['Chris', 'Dani', 'Lucy'];

console.log(students);

//length
console.log(students.length);

//Access an array item
const first = students[0];
console.log(first);
console.log(students[2]);

const last = students[students.length - 1];
console.log(last);

//Loop over an array
students.forEach(function(item, index, array) {
  console.log(item, index);
});

//Add to end of an array
students.push('Karime');
console.log(students);

//Remove from end of an array
students.pop();
console.log(students);

//Remove from the front of an array
students.shift();
console.log(students);

//Add to the front of an array
students.unshift("Chris");
console.log(students);

//Find the index of an item in the array
console.log(students.indexOf("Dani"));

//Remove an item from an indexed position
const items = ["car", "horse", "ball", "house"]
let removedItem = items.splice(1, 1);
console.log(removedItem);
//slice removed the item started at index 1, and removed 1 item.

//Remove an items from an indexed position
const things = ["car", "horse", "ball", "house"]
const removedItems = things.splice(1, 2);
console.log(removedItems);
//slice removed the item started at index 1, and removed 2 items.

// other array methods you should know and practice before class
// .toString()
// .join()
// .includes()
// .indexOf()
// .slice()
// .lastIndexOf()
// .concat()
// .keys()
// .entries()

{% endtonic %}

******

### See It

<!-- Can be a video on youTube as long as it doesn't go to another code school. Eventually all video content should come from ACA. -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/EUnV-fCY0Pc" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Pre-Class Practice: Arrays

#### Instructions

1. Go to the CodePen below, click the top-right corner.
1. Fork it to your account.
1. If not already collapsed, drag the HTML and CSS windows to the left so you're only looking at the JS file.

  <p data-height="265" data-theme-id="0" data-slug-hash="REqBXX" data-default-tab="js,result" data-user="kdybvig" data-pen-title="Arrays Practice" class="codepen">See the Pen <a href="https://codepen.io/kdybvig/pen/REqBXX/">Arrays Practice</a> by Keith (<a href="https://codepen.io/kdybvig">@kdybvig</a>) on <a href="https://codepen.io">CodePen</a>.</p>
  <script async src="https://static.codepen.io/assets/embed/ei.js"></script>

1. [Arrays Practice](https://repl.it/@reneedudley/arraysPractice)
  * Copy this code into a Repl.it and solve for the solutions:

  ```javascript
  //create an array called myName, have each item be a letter of your myName

  //store the length of the array to a variable nameLength

  //add a new item to the end of the myName array. The item should be a string.

  // Remove the last item in myName array and store it's value to an array called deleted letter.

  // reassign the first ite in myName to 's'

  const sentenceArr = [
    ['h','e','l','l','o'],
    ['m','y'],
    ['n','a','m','e']
  ]

  // store the last letter of the first array in sentenceArr to a variable called lastLetter

  //change the 'n' in the last array to an 'N'
  ```

******
******

## Objects

<!-- This is how each subject should be introduced. Give the students structure so they know they can start trusting the process sooner!  -->
[Objects](http://eloquentjavascript.net/06_object.html) are used to store data by unique keys. Objects are different from arrays because they consist of properties and corresponding property values. We refer to these properties and property-values as *key : value* pairs.  Simple rule about creating and object, *keys* must be strings or symbols but the *values* can be any primitive data type or higher order data type.

When accessing values in an object, order does not matter.  For example, to find out what the value of the `id` key of an object is, it would not matter if it was the first key or the three thousandth key, all I would need to access that information is the object and the key name.

```javascript
const exampleObject = {
    name: "Pete",
    age: 80,
    weight: "150 lbs"
    id: 6089,
};

console.log(exampleObject.id) // => 6089
```

### Read it - Creating, Accessing, and Modifying Objects

You can create an object the same way you declare a variable or an array.  Put `{}` around the object's *key : value* pairs then separate each key from it's value with with colons. And at the end of each value place a comma. Check it out below:

```javascript
const person = {
  firstName: "Keith",
  lastName: "Murgic",
  age: 31,
  eyeColor: "brown"
};
```

`person` is is the name of the object. **firstName**, **lastName**, **age**, and **eyeColor** are properties or *keys* of `person`, and the corresponding property *values* are **"Keith"**, **"Murgic"**, **31**, and **"brown"**.

You can access information stored in objects in two ways:

```javascript
// objectName.propertyName
console.log(person.firstName) // => "Keith"

//objectName["propertyName"]
console.log(person["firstName"]) // => "Keith"
```

To change or add a new key/value pair in an object, simply access the value and set it equal to the new value: 

```javascript
person.age = 50` // or person["age"] = 50

console.log(person.age) // => 50

person.birthDate = 1/16/1860
console.log(person) // => {  firstName: "Keith", lastName: "Murgic", age: 31, eyeColor: "brown", birthDate: "1/16/1860" }
```

When build your object remember, keys must be unique, but values can be repeated as many times as needed. The following object would not be a properly formatted object because there are two id keys:

```javascript
{id: 5, name: ‘Renee’, id: 7}
```

This, however, is a properly formatted object
```javascript
{id: 5, name: ‘Renee’, label: ‘Renee’}
```

#### Accessing Nested Data

In real world data, you will see objects with arrays as values and arrays with objects as values, so it’s critical that you can access nested data. Getting good at this is worth the time!!

Let's take a look at the object below:

```javascript
const user = {
    accessCodes: [49303, 493020, 904040, 900404]
    env : ["PA", "NY", "CT" , "VT"]
}
```

Access data one step at a time.  To access the **second item** in the **accessCodes** array, first you need to access the accessCode property then using the return of that first step (which is an array) access the second item in the array.  This can be accomplished two ways:  `user[‘accessCodes’][1]` or `user.accessCodes[1]`. Both ways return: `493020`.

On your own, think about how you would access the **age** property of the second element, **Zuke** in the friends array below. Copy/paste the object into a repl.it and experiment.

```javascript
const user = {
    name: 'Keith',
    friends: [{name: 'Meghan', age: '27'}, {name: 'Zuke', age: '3'}]
}
```

#### Methods of Objects

You can also set a function as a property value. This is when a function is called a method. Anytime a function is put onto an object as a value of one of its keys, it's called a method. :)

```javascript
const person = {
  this.firstName:"Keith",
  lastName:"Murgic",
  age:31,
  eyeColor:"brown",
  talk:  (friend) => {
    console.log("Hello, " + friend)
  }
};
```

The `talk` method is accessed just as any other property on the object, and can be invoked just like any other function:

```javascript
person.talk("Peter")  // => 'Hello, Peter'
```

Speaking of methods, Objects come with their own [built-in methods](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects) and you should look it them for yourself before class! Use the Tonic sandbox below or practice in a Repl.it.

**Experiment with objects below:**

{% tonic %}

const person = {
  firstName: "Keith",
  lastName: "Murgic",
  age: 31,
  eyeColor: "brown",
  talk: function () {
    console.log("Hello!");
  }
};

console.log(person.firstName);

console.log(person["lastName"]);

person.talk();

//practice by creating a new object called "dog" and give it as many key:value pairs as you can think a dog would have

{% endtonic %}

******

#### Major Object Methods you should know

Google each of these and find code samples you can play with in a Repl.it

* .create()
* .entries()
* .assign()
* .keys()
* .is()
* Of course, you should push to learn a new one everyday but these will good ones to start with.

**Let's reiterate the difference between Arrays and Objects once more:**

* Objects are collections of data with **properties** and **property values**.
* Arrays are collections of data with **numerical indexes** for **elements** instead of property names.

******

### See It

<!-- Can be a video on youTube as long as it doesn't go to another code school. Eventually all video content should come from ACA. -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/4uVwGw317QM" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

******

## Pre-Class Practice: Objects

**Instructions**

1. Go to the CodePen below, click the top-right corner.
1. Fork it to your account.
1. If not already collapsed, drag the HTML and CSS windows to the left so you're only looking at the JS file.

  <p data-height="265" data-theme-id="0" data-slug-hash="wRQxoL" data-default-tab="js,result" data-user="kdybvig" data-pen-title="Objects Practice" class="codepen">See the Pen <a href="https://codepen.io/kdybvig/pen/wRQxoL/">Objects Practice</a> by Keith (<a href="https://codepen.io/kdybvig">@kdybvig</a>) on <a href="https://codepen.io">CodePen</a>.</p>
  <script async src="https://static.codepen.io/assets/embed/ei.js"></script>

1. [Object Practice](https://repl.it/@reneedudley/ObjectPractice)
  * Copy this code into a repl.it and solve the problems:

```javascript
//Create an object called testUser. It should have an id of 3.
const testUser = {
  id: 3,
  likes: {
    hiking: 'love hiking'
  }
};
//Add a name key to the object with a value of 'Chris'
// const name = 'renee'
testUser.name = 'Chris';
const hikingValue = testUser.likes.hiking
//Change the name value to 'Christina'
testUser.name = 'Christina'

// likes.drinking= 'loves drinking'

const starChart = {
   locations: [50403, 3030303, 3939303, 303030],
   details: {
     name: 'default star chart',
     date: '03/10/1994',
     location: 'northern hemisphere',
   }
};

const details = starChart.details;
const detailKeys = Object.keys(details);

detailKeys.forEach((key, index)=> {
  console.log(key, details[key])
})

//store the second item in the locations array to a variable called currentLocation
const currentLocation = starChart.locations[1]
//store the name of the start chart to a variable called name;
const name = starChart.details.name;
```

******
******

## Questions for Discussion in the Next Class

You need to google each of these questions and get a grip on what each is hinting at before coming into class. These questions are meant to steer the conversation in class not to be be a lecture from the instructor. If you don't know anything about these topics the instructor will not go over them. Class time is your time to work with an developer to learn *more*.

* What is a function?
* Explain the syntax for functions.
* What are closures?
* How do you use scope when constructing functions?
* Why is it important to consider context in while you build functions?
* What are decomposition method and how do you use them?
* What are fat arrow functions?

## Go to [Classwork >](pigLatinProject.md)

{% include "../includes/footer.md" %}
