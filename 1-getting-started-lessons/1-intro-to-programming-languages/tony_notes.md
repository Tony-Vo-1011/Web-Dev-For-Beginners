# Creating Variables

const => creates unchangable variable
let => changable variable

``` javascript
// Working with objects to group related data
const weatherData = {                       
  location: "San Francisco",
  humidity: 65,
  windSpeed: 12
};
 ```

In the above, we've:

- Created an object to group related weather information together
- Organized multiple pieces of data under one variable name
- Used key-value pairs to label each piece of information clearly

``` javascript
// Modern destructuring for cleaner code
const { location, humidity } = weatherData; 
console.log(`${location} humidity: ${humidity}%`);
```

- assigns changeable variables to constant in one line

# If Else 
``` javascript
// Multiple conditions with logical operators
const userAge = 17;
const hasPermission = true;

if (userAge >= 18 && hasPermission) {
  console.log("Access granted: You can enter the venue.");
} else if (userAge >= 16) {
  console.log("You need parent permission to enter.");
} else {
  console.log("Sorry, you must be at least 16 years old.");
}
```

- Combine multiple conditions using the && (and) operator
- Create a hierarchy of conditions using else if for multiple scenarios
- Handle all possible cases with a final else statement
- Provide clear, actionable feedback for each different situation

``` javascript
// Concise conditional with ternary operator
const votingStatus = userAge >= 18 ? "Can vote" : "Cannot vote yet";
console.log(`Status: ${votingStatus}`);
```

- Use the ternary operator (? :) for simple two-option conditions
- Write condition first, followed by ?, then true result, then :, then false result
- Apply this pattern when you need to assign values based on conditions

``` javascript
// Handling multiple specific cases
const dayOfWeek = "Tuesday";

switch (dayOfWeek) {
  case "Monday":
  case "Tuesday":
  case "Wednesday":
  case "Thursday":
  case "Friday":
    console.log("It's a weekday - time to work!");
    break;
  case "Saturday":
  case "Sunday":
    console.log("It's the weekend - time to relax!");
    break;
  default:
    console.log("Invalid day of the week");
}
```
- Match the variable value against multiple specific cases
- Group similar cases together (weekdays vs. weekends)
- Execute the appropriate code block when a match is found
- Include a default case to handle unexpected values
- Use break statements to prevent code from continuing to the next case