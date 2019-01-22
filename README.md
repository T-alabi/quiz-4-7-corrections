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
```
!=, <, !==, >, <=, >=, ==, ===

```
Question 5: Which of the following are valid logical operators in JavaScript? Select all that apply.

 the valid operators in javascript are as follows: !, ||, &&, 
 
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

# Quiz 7

Question 1: Consider the following code segment.
```
let tripleDigits = numbers.every(function(num) {
   return num >= 100 && num <= 999;
});
```
Assuming numbers has been declared and initialized as shown below, what will be the value of tripleDigits after executing this code?
```
let numbers = [ 101, 202, 303, 4444, 505, 606, 707 ];
```

the value of tripple digits will be true. This is because all numbers are greater than or equal to 100, but letss thaan or equal to 999. 

Question 3:  I have the following array declaration and initialization.
```
let numbers = [ 2, 4, 6 ];
```
I want to add 8, 10, and 12 to the array. Which of the following will achieve that? Select all that apply.

there are multiple ways to add numbers to an an array. You can do this by doing 
numbers.push(8, 10, 12); <br/> numbers[3] = 8;  <br/>
numbers[4] = 10;  <br/>
numbers[5] = 12; <br/>
numbers.push(8); <br/>
numbers.push(10);<br/>
numbers.push(12);<br/>

Quiestion 4: Consider the following code segment.
```
let cars = [ "Audi", "BMW", "Mercedes", "Porsche", "Volkswagen", "Honda" ];
let notGerman = cars.pop();

console.log(notGerman);
console.log(cars);
```
What is printed to the console as the result of executing this code?

```
Honda
[Audi, BMW, Mercedes, Porsche, Volkswagen] 
``` 
the above code will be printed to the console. This is because first logged into the console is consolelog(notGerman) which is equivalent to cars.pop(); which would get rid of the last elemnt in the array honda, and list it first. The  the rest of the array would be listed. 

Question 6: Consider the following code segment.
```
let a = [];
let b = [ 1, 2, 3 ];
let c = [ "a", "b", "c" ];
```
Which of the following represent the contents of each of these arrays? Select all that apply.

a is an empty array. b holds 1, 2 , and 3. and c holds a, b and c. 

Question 8: Consider the following code segment.
```
let cars = [ "Audi", "BMW", "Mercedes", "Porsche", "Volkswagen" ];
let car = prompt("What kind of car do you drive?");

if (/* missing */) {
    console.log("You drive a German-made car.");
}
```
The console.log statement should only execute if the user enters a value that exists in the cars array. Which of the following are possible replacements for /* missing */ that will achieve this goal?

using cars.indexOf(car) !== -1, cars.includes(car), and cars.lastIndexOf(car) !== -1, in the missing section would all work to execute the statemnt. They all only evealute is the desiered value is present in the array. 

Question 12: 
Consider the following incomplete function, which is designed to accept an array of elements and print each one to the screen one-by-one.
```
function printAll(list) {
    /* missing */
}
```
Which of the following can serve as suitable replacements for /* missing */ to achieve the goal of this function? Select all that apply.

the replacements that will be sutiable include: 
```
for (let item of list) {
    console.log(item);
}

for (let i = 0; i < list.length; i++) {
    console.log(list[i]);
}
``` 
this is because both go through the array and print the items on the cosonsole, which is the purpose of the function. 

Question 14: 
Consider the following code segment, which is designed to determine the largest value in an array of integers.
```
function getLargest(integers) {
    let largest = 0;

    for (let integer of integers) {
        if (integer > largest) {
            largest = integer;
        }
    }

    return largest;
}
```
Which of the following sets of test data demonstrates that getLargest does not work as intended?

 the set of data that proves this fuction doesnt work as intended is the one below. This is because none of the negative numbers are greater than zero. 
 ```
 [ -9, -1, -8, -2, -7, -3, -6, -4, -5 ]
```

Question 15: Consider the following code segment.
```
let cars = [ "Ford", "Dodge", "Jeep", "Honda", "Subaru" ];
console.log("I drive a " + cars[2] + ".");
```
What will be printed to the console as a result of executing this code?
I drive a Jeep  will be printed
