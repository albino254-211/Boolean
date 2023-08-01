# Boolean Logic Exercises

# Part I

Write down what the following statements will return. Try to figure this out before putting the commands in the chrome console.

## 1. 2 == "2"; true
- true
## 2. 2 === 2; true
- true
## 3. 10 % 3; 1
- 1
## 4. 10 % 3 === 1; true
- true
## 5. true && false; false
- false
## 6. false || true; true
- true
## 7. true || false; true
- true

# Part II

Answer the following questions about this code block:

## (a)
let isLearning = true;
if(isLearning){
    console.log("Keep it up!");
} else {
    console.log("Pretty sure you are learning....");
}

## 1. What should the above code console.log?
- if(isLearning === true) because the if statement evaluates the truthiness of the expression inside the parentheses. In JavaScript, any value that is considered "truthy" will execute the code block inside the if statement, and any value that is considered "falsy" will execute the code block inside the else statement
## 2. Why do we not need to specify if(isLearning === true)? Why does if(isLearning) work on its own?
- isLearning is a boolean variable with a value of true, which is a truthy value, so the if(isLearning) condition is met, and the code block inside the if statement is executed. If isLearning were false, the code inside the else block would be executed.


## (b)
let firstvariable;
let secondvariable = "";
let thirdvariable = 1;
let secretMessage = "Shh!";

if(firstvariable){
    console.log("first");
} else if(firstvariable || secondvariable){
    console.log("second");
} else if(firstvariable || thirdvariable){
    console.log("third");
} else {
    console.log("fourth");
}


## 1. What should the above code console.log? Why?
- The above code will console.log the message: "third",  because The value of firstvariable when it is initialized is undefined. In JavaScript, when a variable is declared but not assigned a value, it gets the value undefined by default.
## 2. What is the value of firstvariable when it is initialized?
- The value of firstvariable when it is initialized is undefined. In JavaScript, when a variable is declared but not assigned a value, it gets the value undefined by default.
## 3. Is the value of firstvariable a “truthy” value? Why?
- The value of firstvariable is not a "truthy" value.  In JavaScript, "truthy" values are those that evaluate to true in a boolean context. 
## 5. Is the value of secondvariable a “truthy” value? Why?
- The value of secondvariable is an empty string (""). An empty string is also a "falsy" value, so it is not considered truthy.
## 5. Is the value of thirdvariable a “truthy” value? Why?
- The value of thirdvariable is 1, which is a non-zero number. In JavaScript, all non-zero numbers are considered "truthy," so thirdvariable is a "truthy" value.
# Part III
## 1. Research Math.random here and write an if statement that console.log's "Over 0.5" if Math.random returns a number greater than 0.5. Otherwise console.log "Under 0.5".
const randomNumber = Math.random();

if (randomNumber > 0.5) {
  console.log("Over 0.5");
} else {
  console.log("Under 0.5");
}
## 2. What is a falsey value? List all the falsey values in JavaScript.
- A "falsey" value in JavaScript is a value that evaluates to false when used in a boolean context. In other words, these values are considered "false-like" when encountered in conditions, loops, or any situation where a boolean value is expected.