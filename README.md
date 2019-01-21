# Quiz-4-7-corrections

# Quiz 4

 Question: 1 : Consider the following snippet of code.
  let age = 16;
  console.log("age", age);
  What will be logged to the console when this code is executed?

The correct answer for this is age, 16. This is because console.log takes anthing in "quotations" as string or text, so it doesnt read age 
as a varible. When age isnt in quotatons, and still in Console.log it is being referenced to as the varible. 

 Question 3: I want to display a prompt to the user that asks him or her to enter the number of hours he or she worked this week. 
 I would like the default value to be pre-populated with the value 40. I need to store the user's response in a variable named hours.
How can I accomplish this?

the correct answer for this question is as follows: 
let hours = prompt("Enter the number of hours worked this week.", 40); This is because prompts must be set up as prompt(text,defulttext")

Question 6: Consider the following HTML snippet.
<body>
    <button onclick="sayHi()">Click Me</button>
    <p id="my-paragraph">

    </p>
</body>
When a user clicks the button, I'd like to display a friendly greeting. Which of the following JavaScript functions 
(assuming the files are correctly linked) will do the trick? 

there are two ways to display text(basically) and they are setting a varible. like this 
function sayHi() {
    let p = document.getElementById("my-paragraph");
    p.innerHTML = "Hi, there!";
}

or putting it all in one line like so
function sayHi() {
    document.getElementById("my-paragraph").innerHTML = "Hi, there!";
}

Question 7: Which of the following statements declares and initializes a variable called x with the value 27? Select all that apply.

this question asks us to declare the varible beofre we set it equal to anything. So the answer is 
let x; 
x = 27; 

question 9: Which of the following are valid data types in JavaScript? Select all the apply.

The valid data types in javascript are String, null, object, symbol, undefined, boolean and number 

#Quiz 5
