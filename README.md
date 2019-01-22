# Quiz-4-7-corrections

# Quiz 4

 Question: 1 : Consider the following snippet of code.
 ```
  let age = 16;
  console.log("age", age);
  ```
  What will be logged to the console when this code is executed?

The correct answer for this is age, 16. This is because console.log takes anthing in "quotations" as string or text, so it doesnt read age 
as a varible. When age isnt in quotatons, and still in Console.log it is being referenced to as the varible. 

 Question 3: I want to display a prompt to the user that asks him or her to enter the number of hours he or she worked this week. 
 I would like the default value to be pre-populated with the value 40. I need to store the user's response in a variable named hours.
How can I accomplish this?

the correct answer for this question is as follows: 
let hours = prompt("Enter the number of hours worked this week.", 40); This is because prompts must be set up as prompt(text,defulttext")

Question 6: Consider the following HTML snippet.
```
<body>
    <button onclick="sayHi()">Click Me</button>
    <p id="my-paragraph">

    </p>
</body>
```
When a user clicks the button, I'd like to display a friendly greeting. Which of the following JavaScript functions 
(assuming the files are correctly linked) will do the trick? 

there are two ways to display text(basically) and they are setting a varible. like this 
```function sayHi() {
    let p = document.getElementById("my-paragraph");
    p.innerHTML = "Hi, there!";
}
```

or putting it all in one line like so
```function sayHi() {
    document.getElementById("my-paragraph").innerHTML = "Hi, there!";
}
```
Question 7: Which of the following statements declares and initializes a variable called x with the value 27? Select all that apply.

this question asks us to declare the varible beofre we set it equal to anything. So the answer is 
let x; 
x = 27; 

question 9: Which of the following are valid data types in JavaScript? Select all the apply.

The valid data types in javascript are String, null, object, symbol, undefined, boolean and number 

# Quiz 5

Consider the following statements.
```
let x = 43;
let y = "43";

if ( /* missing condition */ ) {
    console.log("x and y have equivalent values and data types.");
}

if ( /* missing condition */ ) {
    console.log("x and y have different values or different data types.");
}
```
Which two expressions satisfy the missing conditions above?

the correct answer to this would be x === y , x !== y. these solutions work because the if functions will evualtuate true and run the code inside the brakets only in these conditions. 

Question 2: Which of the following are valid relational operators in JavaScript? Select all that apply.

the vaild relational operators in java script are as follows:
```!=, <, !==, >, <=, >=, ==, ===
```
Question 5: Which of the following are valid logical operators in JavaScript? Select all that apply.

 the valid operators in javascript are as follows: !, ||, &&, !=, <, !==, >, <=, >=, ==, ===
 
Question 11: Anything written in the form a while (or do...while) loop can be achieved with an equivalent for loop and vice-a-versa.

This is true. Thid is because a do while loop does whatever is inside the brakets as song as it follows the criteria in the while. The for loop does te same thing, instead following the criteria in the set up protion of the loop. 

Question 14: There are four components to the for loop. The initialization (or setup), the conditional expression, the updating of the loop counter, and the loop body itself. What is the order in which these components are executed?

the beging or a forloop is quite simple and con be done in the follwing steps. 
```
1 - Setup  //to begin the loop <br/> 
2 - Expression //simialr to a condition <br/> 
3 - Loop body  // what is being carried out <br/> 
4 - Update //usully the adding of a number to the condition <br/> 
5 - looping back (to step 2)// for the actual looping effect <br/>  
```
# Quiz 6

Question 2: What happens if I pass in more arguments than there are parameters in the function definition? 

if there are more arguments then there are paremeters in the fucntion definition, the function will be retunred undefied. This is because there is more inforamtion then can be stored for the function, therefore, the function cannot be executed correctly and it will return undefined. 

Question 5: Consider the following function, and its subsequent calls.
```
function doSomeStuff(a, b, c) {
   console.log("I need to do " + a + ", " + b + ", and " + c + "... So busy!");
}

doSomeStuff("homework", "chores", "more homework");
doSomeStuff("chores", "homework");
doSomeStuff("homework", "homework", "more homework", "oh, and chores, too");
Select the statements that will be logged to the console. Choose all that apply.
```
This will be: I need to do chores, homework, and undefined... So busy! //because c has to defined value <br/>
I need to do homework, chores, and more homework... So busy! //all varibles defined <br/>
I need to do homework, homework, and more homework... So busy! //all varibles defined <br/>

Question 9: Consider the following function.
```
function divide() {
    let a = Number(prompt("Enter a number."));
    let b = Number(prompt("Enter another number."));

    return a / b;
}
```
I want to modify the function so that it accepts as parameters the values being divided. Which of the following revisions achieves this?

The answer to this would be: 
function divide(a, b) {
    return a / b;
} 
there would be no need to re define to parameter varibles (a & b) as prompts and numbers, becuase theyre defined as paremeters. 

Question 10: Which of the following built-in functions are designed to return a value? Select all that apply.

prompt is a built in function that is designed to retunr a value. It returns the users input, even if it is null. 

Question 14: Consider the following code snippet.
```
function example(a, b, c) {
    if (a === 1) {
        if (b === 2) {
            if (c === 3) {
                var d = 4;
            }
        }
    }

    console.log(d);
}
```
What is the result of executing this code?

4 or undefined will be printed to the console. 4 will be printed only if a = 1, b = 2, and c = 2. 
It will return undefined if one those values is not true. 
