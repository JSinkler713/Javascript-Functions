# Javascript Functions

## Lesson Objective:
**To declare and call functions in JavaScript**

## This is how we have declared *variables* up to now:
    var name = 'bob';
    let animal = 'dog';
    const time = 'now';
## This is how we declare *functions*:
```javascript
    function sayHi() {
      return 'Hi'
    }
```

Instead of *var* *let* *const* we use ***function***  and then an identifier, in this case `sayHi`. To tell javascript we are making a *function*  we need to pu parenthesis`()` after the identifier. This parenthesis is for anything we want to pass into the function. In this case we don't put anything in the parenthesis. The rest of the function --what we want the function to do-- we put in curly brackets `{}`. A function will always ***return*** something, in this case we have it return the string 'Hi'.
## Lets take a second to put the above code in our console in an open web-browser

To open up your dev-tools in chrome the shortcut is  `option` `command` `j`

To open up your dev-tools in firefox the command is `option` `command` `k`

## Great we just declared a function!
Congratulations you are on your way to being a developer. Functions are how we tell the computer to do things. Html and Css can put words on a page and style them, but if we actually want our user to interact with a page, we need JavaScript functions.

-So how do we call a function?

## To call a function:
Go ahead and type this in your console:
    `sayHi`

Talk to the person next to you, did it do what you thought it would? What do we know about sayHi?
<details>
  <summary>To call a function...</summary>


We need to go ahead and type these all important `()`  in our code. So now type in `sayHi()` and see what we get
</details>

## Ok, now we are going to make a function that takes in a *parameter*. This is a placeholder for an actual value or *argument* we will pass in.
![image of function diagram](function.png)

If we want to change our `sayHi` function to say hi to a certain person, we would want to be able to pass in different people's names. To do this we edit our function a little bit. I'm going to call this new function `sayHiTo` .

```javascript    
    function sayHiTo(name) {
      return 'Hi ' + name
    }
```

Our *parameter* or *placeholder* in this case is *name*. We can pass in different *arguments* or *actual values* in it's place when we call our function.

Say this 5 times fast: 'A parameter is a placeholder. An argument is an actual value. Parameter - placeholder. Argument - actual. Parameter - placeholder. Argument - actual.

Ex:

```javascript
    sayHiTo('James');
```

Here we pass in the *argument* 'James'. So put this in yor console and pass in the *argument* to say hi to your neighbor.

---
## Your turn:
Click [here](javascript-functions-assignment.js) to open a short assignment. Take a minute to try and *declare* and *call* the two functions. For now we can just type the code in the console for test purposes. We will go over the solution in a minute. Try it on your own first, then reach out to a partner or myself if you can't get it working. 


<details>
  <summary>Solution</summary>

    // Write a function that has two parameters and sums them together
```javascript
    function addNums(x, y) {
    //write your code here
      return x + y;
    //DON'T forget to return the value
    }


    //call the function with the arguments 3 and 5
    addNums(3, 5)  // returns 8

    //************************************************************
    // Declare a function greetFrom(), that has a parameter name, that then returns 'Greetings from <whatever name is passed in>'
    function greetFrom(name) {
      return 'Greetings from ' + name;
    }

    // Call the function passing in your own name as an argument
    greetFrom('James') // returns 'Greetings from James'

```

</details>

## Questions?

---
## A few other ways we can make functions in case you see them out in the wild.

```javascript
    //This is a function expression
    var subtractNums = function(numOne, numTwo) {
      return numOne - numTwo
    }

    //This is an arrow function
    const Party = (partyPerson) => 'Wooohoo ' + partyPerson + '!!'
```
## RECAP
Javscript function decleration:

```javascript
    function mysteryFunction(paramOne, paramTwo) {
      return paramOne / paramTwo
    }
```
Pop this into your console, and then ***call*** the function with two **arguments** that will *return* the value 4.

Note: There are many correct answers

<details>
  <summary>Here's one</summary>

  `mysteryFunction(20, 5) // It is a division function`

</details>
