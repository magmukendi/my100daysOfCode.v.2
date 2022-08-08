# my100daysOfCode
<h4> In this repository I document my journey for the 100 days of Coding challenge</h4>

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
**Link to work**: The project 1 can be found [here] (https://github.com/me50/LeGrandMAG/tree/web50/projects/2020/x/wiki)


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
 - Space complexity: how much space the algoruthm takes in our memmory. Recursive binary search is O (log N). 
 
 Need to look into Tail optimization for more details.
 
 **Thoughts**:I came accross a great way to measure efficiency of things while coding or even in real life. We use the worst case scenario as a bench mark for our expectation. I think learning algorithm is very helpful for me.
 
 
  **Link to work**: my work can be foun at [this repo](https://github.com/LeGrandMAG/Data-Structures-and-Algorithm)



## Day 50/100 July 25 2022:

## Day 49/100 July 24 2022:
 - Started working on a auctions website
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

