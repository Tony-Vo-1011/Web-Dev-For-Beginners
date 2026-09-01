``` javascript
function nameOfFunction() { // function definition
 // function definition/body
}
```
Let's break this down:

- The function keyword tells JavaScript "Hey, I'm creating a function!"
- nameOfFunction is where you give your function a descriptive name
- The parentheses () are where you can add parameters (we'll get to that soon)
- The curly braces {} contain the actual code that runs when you call the function


``` javascript
function displayGreeting() { 
    console.log('Hello, world!');
}
```
``` javascript
// calling the function
displayGreeting();
```
This executes the code inside displayGreeting function and prints "Hello, world!" in browser's console

``` javascript
function createGreetingMessage(name) {
  const message = `Hello, ${name}`;
  return message;
}
```
Now instead of printing the greeting, this function creates the message and hands it back to us.

To use the returned value, we can store it in a variable just like any other value:

``` javascript
const greetingMessage = createGreetingMessage('Christopher');
```

Now greetingMessage contains "Hello, Christopher" and we can use it anywhere in our code – to display it on a webpage, include it in an email, or pass it to another function.

Functions can be passed as parameters for other functions. setTimeout is a built in function that waits for a certain amount of time then runs some code. We need to tell it what code to run.

``` javascript
function displayDone() {
  console.log('3 seconds has elapsed');
}
// timer value is in milliseconds
setTimeout(displayDone, 3000);
```
When passing functions into other functions, no parentheses are needed.

Anonymous functions are functions needed for just one thing so you don't want to bother with a name

``` javascript
setTimeout(function(){
    console.log('3 seconds has elapsed');
}, 3000)
```

More modern and concise syntax uses the fat arrow. The same code could be written as:

``` javascript
setTimeout(() => {
    console.log('3 seconds has elapsed');
}, 3000)
```