# my100daysOfCode
<h4> In this repository I document my journey for the 100 days of Coding challenge</h4>


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

