# my100daysOfCode
<h4> In this repository I document my journey for the 100 days of Coding challenge</h4>

## Day 90/100 September 3rd 2022:
### **Today's Progress**: No coding, resting

## Day 89/100 September 2nd 2022:
### **Today's Progress**:
https://www.tecmint.com/open-source-api-gateways-and-management-tools/
I already passed 11 out 12 tests for the random Quote Machine.
Finally finished the Random quote machine.

### **Thoughts**: GIven that we are planning to have a beta test sometime this week, I will be working the app UI until today.


## Day 88/100 September 1st 2022:
### **Today's Progress**:
https://www.tecmint.com/open-source-api-gateways-and-management-tools/
I already passed 11 out 12 tests for the random Quote Machine.
Finally finished the Random quote machine.

## **Thoughts**
## **Link**: 
[Random Quote Machiine](https://codepen.io/legrandmag/pen/xxWvBvp)
## Day 87/100 August 31st 2022

https://www.yapp.co.kr/project/20th/betree
### **Today's Progress**:

**TASK 1: Mapping the state and action creators to props**

We will access specific states and actions by using the function mapStateToProps() and mapDispatchToProps().

And We will use those two functions with the react redux connect() method to connect the state and the  to the components.


- In order for us to use the function mapStateToProps(). We use the argument state and return an object with property messages mapped to the state.


- In order for us to use the function mapDispatchToProps(). We use the argument dispatch.
It returns an object that map the different actions creator to use in the component. We returns a function.



**Task 2: Connecting state and dispatch to component**

Now that I know how to use the mapStateToProps() and the mapDispatchToProps(). I can connect them to the component using the React redux connect() method as following.


```
const connect = ReactRedux.connect
const ConnectedComponenet = connect(mapStateToProps, mapDispatchToProps)(Presentational)
```

When we make a component that do not interact with any redux, we called them Presentational component and the component that connect with the redux is called Container component.


**Task 3: Extract local state into Redux**
I was able to extract the local state and add it into my Redux

#### Final Projects


1. Random Quote Machine



### **Thoughts**: 

I was able to combine react challenges from free code camp and Scrimba, and I finally finished all the challenges. I just need to work on the final projects and build usefull stuff.

### **Link**:
[Random Quote Machiine](https://codepen.io/legrandmag/pen/xxWvBvp)


## Day 86/100 August 30th 2022:

**Today's progress**: I am still working on Redux. I started enforcing immutability of state in redux. 

We usually just spread the array so that to habe a new cloned array.

**TASK 1: Adding an element in a array without modifying the array**.
. 
We just  spread the array, add a comma and add the new element. 

*e.g ```[...state, action.todo]```*
In this example the ***state*** is  the array we clone and ***action.todo*** is the new element we add to the array. 

**TASK 2: Removing an item from an array in a state**.

In order forus to be able to remvoe an element from an immutable state. we can use the slice. 
Let's say we have the following array [0,1,2,3,4,5,6,7] and we would like to get rid of 5 ( which has and index of 5). We will do the following.

```[...array.slice(0,5),...array.slice(5 + 1,array.length)]```

The code above will first return the array from 0 to 4. Notice that when we use the slice() method the first argument is the starting index and the last argumen is the last argument is where the slice should end ( excluding the index). And the second element after the comma is what we will add to the spread operator. We will start the slice one index after the element we would like to remove (index + 1) and we would add till the end of the array (array.length).


**TASK 3: Working with state as object**. 

When working with object we can use Object.assign(). We use it to copy the property of object ( in the second argument) into an empty object in the first argument. The 3rd argument is the object that need to will overwrite any property contained in obj2.


e.g  ```const newObject = Object.assign({}, obj1, obj2, obj3 )```. This will create a new oobject with the property in obj1, obj2, and obj3



**TASK 4: React and Redux**.

**Thoughts**: I just finished the module about redux. Now I will have to combine React and Redux.


How to use react-redux.

React-redux has  two key features: Provides and connect.

Provider: is a wrapper component from react redux that wraps the react app. It takes two props. The redux store and the child component of the app.
In order for us to combine the react and redux we use the provider.

It looks like this:

```
<Provider store={store}>
  <App/>
<Provider/>
```

**Thoughts**: It was super nice to try to build something using redux and react at the same time.
**Link to work**:

## Day 85/100 August 29th 2022:

**Today's progress**: 
TASK 1: Sending action data to the store

TASK 2: Using middleware to handle asynchronous actions
 Redux has middle that helps us handle asynchronous endpoints. Redux Thunk middleware.
 
TASK 3: Making a counter with Redux
**Thoughts**: I still need to review the redux thunk middleware. It is a little more complex. I did not fully comprehend the use of store.dispatch() so I will come back to that later for more practice.
**Link to work**: Still no link available. I will share link to real projects when I finish this module.


## Day 84/100 August 28th 2022:
**Today's progress**: 

Task 1: Worked on Redux reducer. A common practice while working with reducer is to use const for action types. It is better to use constant rather using strings.

Task 2: I also learned how to use the subscribe() method from the redux. I got an hand on dispatch functions. Which is like a way for us to listen to change made in the store.


Task 3: Combine multiple reducers. When the app starts to grow bigger and bigger, it is temptiing to divide its state to multiple pieces. But if you use redux, you should keep them in a single state object. You should have a root reducer and pas that it into the redux createStore() method.

For us to be able to combine multiple reducers, we can use the combine Reducers() method. It is best practice to create a reducer for each of the application state when they are distinct or unique.



For ex. Note taking app with user authentication, one reducer can handle authentication and another could handle text and notes that the user is submitting.

we will write a combineReducers() 

const rootReducer = Redux.combineReducers({
auth: authenticationReducer,
notes: notesReducer
})


**Thoughts**: I am just getting used to redux and I can see how very practical it is for bigger and more complex project. I still did not fully explore its applicability but I am looking forward to start using it in my React projects.
**Link to work**: There isn't any relevant link for this module. I will share the link


## Day 83/100 August 27th 2022:
**Today's progress**:
**Thoughts**:
**Link to work**:

## Day 82/100 August 26th 2022:
**Today's progress**:
**Thoughts**:
**Link to work**:


## Day 81/100 August 25th 2022:

**Today's Progess**: I am finally finishing the cash register. 


**Thoughts**: The logic behind the code itself was easy but. I forgot one important programming principles: divide and conquer. I was trying to solve the problem having the bigger picture in mind. The best solution was to break every single problem in small tasks and solve them one after the other. I swear I did watch other people's work.

**Link to work**:
- [Cash Register](https://github.com/LeGrandMAG/freeCodeCamp/blob/master/Intermediate%20Algorithm%20Scripting/finalProjects/cashRegister.js)


## Day 780/100 August 24th 2022:
**Today's Progess**: Today was such a busy day. I barely touched my PC to code.
**Thoughts**: Nothing much to say here.
**Link to work**:
- [Cash Register](https://github.com/LeGrandMAG/freeCodeCamp/blob/master/Intermediate%20Algorithm%20Scripting/finalProjects/cashRegister.js)


## Day 79/100 August 23rd 2022:
**Today's Progess**: I am still working on the cash Register. I did not finish it yet :(. I cannot manage to pass the last code test. The test asks me to return unsufficient found if the change in the drawer is less than the change due. But this is super confusing.
**Thoughts**: NOthing much to say here.
**Link to work**:
- [Cash Register](https://github.com/LeGrandMAG/freeCodeCamp/blob/master/Intermediate%20Algorithm%20Scripting/finalProjects/cashRegister.js)

## Day 78/100 August 22nd 2022:
**Today's Progess**: 

I finished working on the US Telephone Number validator. A program that check if the inputed number is a valid US phone number.

I finished working on the Roman Numeral Converter. A program that convert any given number into Roman Numeral notation.

I finished working on the Caesars Cipher also known as the shift cipher. It is a program that shift the value of letters 

**Thoughts**: This project was quite easy to achieve. I just needed to find the right algorithm to apply. I just noticed that it is easier for me to work with algorithm that include strings and characters rather then surface or spaces as it is the case in many of code tree problems.

**Link to work**: 
- [Roman Numeral Converter](https://github.com/LeGrandMAG/freeCodeCamp/blob/master/Intermediate%20Algorithm%20Scripting/finalProjects/romanNumeralConverter.js)
- [Caesars Cipher](https://github.com/LeGrandMAG/freeCodeCamp/blob/master/Intermediate%20Algorithm%20Scripting/finalProjects/caesarsCipher.js)
- [Telephone Number Validator](https://github.com/LeGrandMAG/freeCodeCamp/blob/master/Intermediate%20Algorithm%20Scripting/finalProjects/telephoneNumberValidator.js)

## Day 77/100: August 21st 2022:
**Today's Progress**: I worked on the Map Debris, a program that computes thev orbital Period using Kepler's Third Law.

I also finished working on the Palindrome Checker, it is one of the 4 projects to finish Javascript Algorithms and Data Structures Projects. This project check for work that are identical forward and backward after removing all the alpha-numeric characters such as comma space and symbols and converting everything into lowercase.


**Thoughts**: I finally finished all 21 challenges about Intermediate Algorithm Scripting in the Javascript Algorithms and Data Structures from free Code Camp. I only have to complete the 4 projects left and I will get my certificate.  

**Link to my work**: 
- [Map the Debris](https://github.com/LeGrandMAG/freeCodeCamp/blob/master/Intermediate%20Algorithm%20Scripting/mapTheDebris.js)
- [Palindrome Checker](https://github.com/LeGrandMAG/freeCodeCamp/blob/master/Intermediate%20Algorithm%20Scripting/finalProjects/palindromeChecker.js)

## Day 76/100 August 20th 2022:

**Today's Progress**: 
 - I worked on Make a Person. A program that creates an object that take as argument the full name, create methods that log the first name, the last name, the full name. Methods that update the first name, the last name, the full name.
 
 - I also worked on WEPO App's frontend design. I started working on the product page. Which will contain the different post of the application. I was having some issues with with adding a sticky effect CSS's position stucky effect for the text field when people search for item on the posting page. Also if someone try to click on loop icon, instead of being redirected to the search screen, he would stay at the product list screen and to the query from there. Also, when someone does a query but there is not result for the query, He should see a component telling him that there is no search results.


**Thoughts**: I think this program might be very useful when I am building form or I am trying to register people in a Data base.

**Link to work**: [Make a Person](https://github.com/LeGrandMAG/freeCodeCamp/blob/master/Intermediate%20Algorithm%20Scripting/makeAPerson.js)

## Day 75/100 August 19th 2022:
**Today's Progress**: I worked on Arguments Optional. I had to build a function that takes two arguments and return the sum. In case only one argument was given, it will return a function that take another argument  And return the sum of both arguments. If we input an argument who type is different from number, the code should return the sum of both the arguments.
**Thoughts**:
**Link to work**: The work can be found [Arguments Optional](https://github.com/LeGrandMAG/freeCodeCamp/blob/master/Intermediate%20Algorithm%20Scripting/makeAPerson.js)

## Day 74/100: August 18th 2022: 

**Today's Progess**: I worked on Code Treee challenges.
**Thoughts**:
**Link to work**

## Day 73/100 August 17th 2022:
**Today's Progess**: I worked on Code Treee challenges.
**Thoughts**:
**Link to work**

## Day 72/100 August 16th 2022:

**Today's Progress**: I practiced some intermediate algorithm in Javascript. I worked on a program that check if all the  a property is truthy in all the objects of the list. Instead of using the traditional Boolean(), i designed a function that check for all that and return true or false value.


**Thoughts**: I think the project doesn't really have any use cases but I think it was super important to understand the logic behind that.

**Link to work**: The work can be found here:[Intermediate Algorithm Scripting](https://github.com/LeGrandMAG/freeCodeCamp/tree/master/Intermediate%20Algorithm%20Scripting)


## Day 71/100 August 15th 2022:

**Today's Progress**: I revisited Redux. Reviewed how to use redux store. 

***Redux action**: A redux action is just an object with type. 

**Redux action creator**: In order for use the define a redux action creator. we just need to define a function that return an action,

**Redux dispatch method** is used to dispatch actions to the reduc store.
**Thoughts**: I wasn't really sure about why I should using redux, but after understanding that it is pretty hard to manage state on their own, redux becomes a very usefull tool.
**Link to work**: [Free Code Camp: FrontEnd Development Libraries (redux)](https://www.freecodecamp.org/learn/front-end-development-libraries/#redux)

## Day 70/100 August 14th 2022:
**Today's Progess**: 
**Thoughts**:
**Link to work**:


## Day 69/100 August 13th 2022:

## Day 68/100 August 12th 2022:

## Day 67/100 August 11th 2022:

## Day 66/100 August 10th 2022

## Day 65/100 August 9th 2022:

## Day 64/100 August 8th 2022:

## Day 63/100 August 7th 2022:

## Day 62/100: August 6th 2022:
**Today's Progress**: I am currently reviewing dx/dy technique. How to move a point in a grid. I also worked on how to change the direction of the point in a plan. 
When working with grid it is always important to mention the out of range bound. So that you can can be protected from being out of range.


**Thoughts**: 
**Link to work**:



##Day 61/100 August 5th 2022:

**Today's Progress**: 
**Thoughts**: 
**Link to work**:

##Day 60/100 August 4th 2022:

**Today's Progress** :  
**Thoughts**: 
**Link to work**:

## Day 59/100 August 3rd 2022:

**Today's Progress**: 2차원 배열. Which is like a 2d array. I got to learn that when we use the ```len()``` method in a 2d array it return the number of rows. Also I was today's year old when I discovered that I can also use the following formula to add elements into an 2d array.

```
arr = [
 list(input().split())
 for _ in range(3)
 ]
 ```
 I also worked on the intermediate algorithm from freeCodeCamp. I worked on a **DNA pairing, missing letters** program.
 
**Thoughts**: 
**Link to work**:

## Day 58/100 August 2nd 2022:

**Today's Progress**: Today I worked on on codetree's assignments. 1차원배열, 2차원 배열, and 문자열 전부
**Thoughts**: After working on those assignments I feeel more confident about my python coding. It is true that practice makes perfect.
**Link to work**:

## Day 57/100: August 1st 2022:
Worked in freecode camp's Javascript intermediate algorithm.



## Day 56/100: July 31 2022:
Worked on the codetree questions. Reviewed input and output in python,.



## Day 55/100: July 30 2022

**Today's Progress**: I worked on codetree problem for novice low. I think I will be done very soon.This level focus on printing. 출력. IN order for me to print something on python I will need to use one of those three ways:

```
print("")
print(f"")
or print({}.format{})
```
**Thoughts**: It is always great to start back fresh again. I am just 
**Link to work**: I ma not having a seperate link to document my progress. When I start working on harder algorithm questions. I will update that.


## Day 54/100 July 29 2022:

**Today's Progress**: Today I worked on cs50 project again. I finished the project 1 (wiki). Hopefully I will get a reply very soon. This project taught how to use filtering. and playing with the views in django.
Built a piano notes playing app.
**Thoughts**:  I is very hard to code and to programming and one of the best thing we can do is to find a supportive community.
**Link to work**: The project 1 can be found [here](https://github.com/me50/LeGrandMAG/tree/web50/projects/2020/x/wiki)


## Day 53/100 July 28 2022:

**Today's Progress**: Today I worked on the cs50's web programming with Python and Javascript.
I was working on the week 4 The content was about SQL, Models, and Migrations(project 2). I also reviewed some command to create a table.

** CREATE TABLE **

For us to work with table we need to add a primary key to each table (and it should AUTOINCREMENT). Also we need to have constraints (for e.g NOT NULL, DEFAULT, UNIQUE, PRIMARY KEY, CHECK check if a value is within a specific range) for different elements of the table.

A normal table will look like this:

```
CREATE TABLE flights(
id INTEGER PRIMARY KEY AUTOINCREMENT,
origin TEXT NOT NULL,
destination TEXT NOT NULL,
durartion INTEGER NOT NULL
);
```
BUt how do we add data in that table? We will use the command INSERT INTO as folow:

```
INSERT INTO flights
(origin, destination, duration)
VALUES("New York", "Kinshasa", 415);
```
For us to retrieve the data from the table we use the select/
```
SELECT * FROM flights;
```

or ```SELECT origin, destination FROM flights```

For us to be able to update a datav in a table we use the  command UPDATE:

```
UPDATE flights
SET duration = 430
WHERE origin = "Kinshasa"
AND destination = "London";
```
For us to be able to delete data we use DELETE:

```DELETE FROM flights WHERE destination = "Kinshasa";```

The are also some other clauses: such as LIMIT, ORDER BY, GROUP BY,  HAVING, and many more

What is a foreign key ?

When our table have a lot of data it becomes messy. In order to fix that we need to make new simpler table and use foreign key to reference to them.

**Thoughts**: I think cs50 is very helpful. The way they teach the examples, the exercises, the Project. That is amazing.
**Link to work**: No link available.

## Day 52/100 July 27 2022:

**Today's Progress**: To I specifically focused on the sorting algorithm. I learned about LinkedList and the merge sort algoroithm.

**Thoughts**: I was thinking that Data structures and algorithms was super hard. But learning the Data structures, with good explanation I am able to understand very well.

**Link to work**: my work can be foun at [this repo](https://github.com/LeGrandMAG/Data-Structures-and-Algorithm)


## Day 51/100 July 26 2022:

 **Today's Progress**:
 - Worked on algorithms: Binary search and linear search
 - Reviewed algorithm time complexity. How much time an algorithm takes to complete a t
 - Space complexity: how much space the algorithm takes in our memmory. Recursive binary search is O (log N). 
 
 Need to look into Tail optimization for more details.
 
 **Thoughts**:I came accross a great way to measure efficiency of things while coding or even in real life. We use the worst case scenario as a benchmark for our expectation. IF we consider the worst case scenario we can prepare for it and plan accordingly. Even though it does not happen, at least we would know that the we are safe.
 
 
  **Link to work**: my work can be found at [this repo](https://github.com/LeGrandMAG/Data-Structures-and-Algorithm)



## Day 50/100 July 25 2022:

## Day 49/100 July 24 2022:
 - Started working on a auctions website as part of the cs50 Web Programming with Python and Javascript's project.
## Day 48/100 July 23 2022:

## Day 47/100 July 22 2022:

## Day 46/100 July 21 2022:

## Day 45/100 July 20 2022:


**Today's progress**: few days ago I started working on the email system, followigg CS50w's email system. And i think i was able to solve the first question. Which was about allowing the user to fill out an email and send it to the API using the post request.

I also worked on reviewing my understanding of Redux. Redux will help us to store component states. 

We can use `getState` to get the state stored in the redux store.
I learn about the method createStore(). It take a reducer as a required argument.

We also use Reduc to update the state. To do that we use actions, Redux actions are a js object that contains in fomrn

**Thoughts**: I spent about 3 days figuring out how to do so that I am able to send a post request to the API. But I just noticed that, the biggest problem was not about the post request but the way I was trying to submit the form.


I was using  `document.querySelector('#compose-send').onsubmit` and this was selecting the button and trying to submit. Which is a mistake. Instead i should have used `document.querySelector('form')onsubmit` in order to select the form and submit the form.

***Link to work***: 
the link to my work can be found [HERE](https://github.com/LeGrandMAG/cs50w-mail)


## Day 44/100 July 19th 2022:
Worked on a wordle game:

***Today's progress***: I finally finished Bob Ziroll React Course on Scrimba. I was just going over all the work I have done and also watch some interview questions and see if can handle them. The result is quite not bad at all. I think I can stand for few minutes during the interview.


**Thoughts**: My thoughts are that even though it is taking me some time to figure out how to do things, I still manage to get it done and that is the most important thing.

I would not be attaching anylink got my work today.


## Day 43/100 July 18th 2022 (Monday):

 **Today's Progress**: I worked on the Tenzi game, I worked the game from the beginning till the end. I also learned how to use react-confetti, when the user has won the game.
 After completing the project, here are some extra features, I can add to the game:
   - Put real dots on the dices.
   - track the number of rolls it took to win
   - track the time it took to win.
   - Save the time it took to win to local storage.
   
 **Thoughts**: I think it is very important to start with the main feature of the platform. And then add additional features.
 
 **Link to work**: the code can be found at my project on [Sandbox code](https://codesandbox.io/live/1fa25d918e3)




## Day 42/100 July 17th 2022:
- today I worked on WEPO's landing page: I updated the nav bar and the footer component. The hero component is in progress.
- I also worked on the Memory game. The user will flip a card and be able to compare two card.



## Day 41/100 July 16th 2022:

- worked on a email service as the project 3 of CS50 W for web development
- watched interview questions
- worked on WEPO's project by review codes.


## Day 40/100: july 15th 2022:
 - Worked on useEffect cleanup function
 - Worked on the toggle dark mode / light mode
 - working on the markdown editor on 
 - how to use localStorage
 -  localStorage uses .getItem("key) to get the item stored in the local storage and use setItem("key", value) to save something in the memory.local storage contrary to the sessionStorage has no expiration time. But if you use it in a private or incognito mode the data are cleaned when the last tab is  closed. Also the value need to be stored in string, not array, object.
 -  You can use JSON.stringify(value) to conver the value into string. And use JSON.parse(stringifiedValue) to convert it to its original type.
 
 
 
 Aditionally I registered for the Samsung Collegiate Programming Cup. It is mostly based on alrgorithm and data structures. I will be spending today and tomorrow's on understanding more about alrogithms to get prepared enough for the Cup.
 
 Sources I was suggggested: The Algorithm Design Manual, Interactive python algorithms website, practice website such as coderbyte and hankerrank,topcoder, codervyte, project euler,hackerrank,codechef, exercism.io, codewars, leetcode, spoj, codingame, read algorithms explanation from geeksforgeeks.
 
 


coding interview

## Day 39/100 July 14th 2022:
- Worked on a meme Generator.
- Intro to Redux.
- More Data Structures and Algorithms in JavaScript.




## Day 38/100 July 13th 2022:
 - dependency array
 - API Call
  - worked on looping through API elements.
 - worked on WEPO's price calculator web app.



## Day 37/100 July 12th 2022:
- worked on side effect. The side effect check for any update in the component and then run the callback functions inside it.

- React cannot interact with local storage, API database interactions, subscriptions (web sockets), syncing different internal states,


## Day 36/100 July 11th 2022:

- Today I worked on boxes display on react. I built a component that check for check if a box is on or off. If it is off I added a toggle to toggle the box on. If it was on I added a toggle to toggle the box off.
- I also worked on a component that shows joke. It displays a joke and when the user click a button it toggle the punchline on.
- Worked on a component that tells how many unread messages I have in case I have more that 0 unread messages. Change the word messages to message in case I have only one unread message. And display "You are all caught up in case I have 0 unread message. ***Conditional rendering***
- I also started working on forms in React.
- Worked on controlled component to manage use input in forms.
- I also started working on lifecycle method (componentWillMount, componentDidMount, shouldComponentUpdate, componentDidUpdate)
- Worked on a magic height ball project on react.
- Age verification system using thernary operator.
- Rendering on the Server

## Day 35/100 July 10th 2022
Today I did not code I spent most of the time reading, meeting and resting.
## Day 34/100 JUly 9th 2022
Today I worked on react project to creat a meme generator
## Day 33/100 July 8th 2022

Today I was working on a react projects. I learned conditional rendering using react. Event listener and side effect.
I got to practice how to interact with element on the DOM using event listener on React.

## Day 32/100 July 7th 2022

More Data structure and algorithms in Javascript.
- Today I learned about how to use map() for rendering elements such as list of products, list of posts and more.

## Day 31/100 July 6th 2022
Functional programming. How to name variables, what tyo do to keep the variable name up to the industry standard.

## Day 30/100 July 5th 2022

- Imperative code. Instead of using for loop we can use map().
- in functional programming changing  things is called mutation and the outcome is called side effect.
- We use map() as a replacement of for loop or ForEach.
- We use filter() to select specific element that meet a certain standard.
- We use reduce() to compute the sum of elements.
- We use sort(). And we need to always remember callback functions comparedFunction while using sort() method.
- We will use split() to  convert a string into an array
- We will use join() to convert an array into a string.

In  today's challenge we tried to convert a string into a url slug. With such a simple formula. 
```function urlSlug(title) {
title = title.toLowerCase()
return title.split(/\W/).filter(item => item !== '').join('-')
```
 - We also learn how to use the "every" method. We use it to check if all the element of an array satisfy a condition in the callback function and return true or false.
 - We use some() to check if any of tghe element in an array satisfy a condition and return true or false.

Also learned about currying an partial application.

Arity of a function is the number of arguments it requires. Currying a function means we convert a function of N arity into N functions of arity 1. We restructures a function so it takes one argument.
Currying a function is useful if you cannot supply all arguments to a function at one time. 

Partial application...DID NOT REALLY GRASP THIS CONCEPT

**Now I just started working on the Intermediate Algorithm Scripting Challenge**

## Day 29/100 July 4th 2022
- Today I am working on Immediately Invoked Function Expression (IIFE). 
- At first I did not know that you can actually declare a function and call it on the spot, But thanks to this challenge from freeCodeCamo, I was able to learn that.  It is actually pretty easy  to understand.
- I am at the last challenge about the OOP in JavaScript. If I finish this, I will get into functional programming, I hope it will be very resourcefull for my future projects.
- I am also learning callbacks ( functions that are slipped or passed into another function to decide the invocation of that function.
- First class functions are functions assigned to variable, passed as parameter of other function or returned from another function just like any other normal value. callbacks are also first class function.
- Function tha take a function as a parameter or return a function as a return value is called higher order function.

## Day 27 and 28 July 2nd and July 3rd 2022
- Today I worked on the importance of Data Structures and Algorithms in Javascript. 
- And I also worked on some coding challenge and watched some React coding interview for beginner coding with Clement the founder of AlgoExpert.
- I also learn how to construct an object, how to make chikd object inherit from it parent object and how to use prototype to make more objects. And finally how to build prototype of unrelated objects using mixin.

