# FizzBuzz Documentation
I started by referring to lines 71 to 76 of the codealong.js file in the [04ControlFlow subfolder](https://github.com/rdwrome/261sp25/blob/main/04ControlFlow/codealong.js), which depcited code for finding numbers divisible by 7 and 5 between 1500 and 2700. I altered the code slightly so the counter would start at 1, count up to 100, and check to see if the number was divisible by 3 and 5. Instead of printing the number, I wanted the word FizzBuzz to be printed so I put this in the parenthesis following console.log. I then added if statements to account for the numbers that were only divisible by 3 and numbers that were only divisible by 5. For the numbers only divisible by 3 I used console.log(Fizz), and for the numbers only divisible by 5 I used console.log(Buzz). 

`
for (let i = 1; i <= 100; i++) {
   if (i % 3 === 0 && i % 5 === 0){
     console.log(FizzBuzz);
  }
  if (i % 3 === 0){
    console.log(Fizz)
  }
  if (i % 5 === 0){
    console.log(Buzz)
  }
  }
`
After checking the above code using the Eloquent JavaScript code sandbox, I realized that I needed to use quotes for the words I wanted to print. After implementating the quotation marks for the words "FizzBuzz", "Fizz", and "Buzz", I once again checked my code with the sandbox and realized none of the numbers were being printed. I implemented this in an else statement at the end of my code.

`
for (let i = 1; i <= 100; i++) {
   if (i % 3 === 0 && i % 5 === 0){
     console.log(FizzBuzz);
  }
  if (i % 3 === 0){
    console.log(Fizz)
  }
  if (i % 5 === 0){
    console.log(Buzz)
  }
  else {
    console.log(i)
  }
  }
`
After checking this code once again, numbers and words were being printered; however, there were still errors in the printed list. I referred to the codealong.js file again and realized I needed to use else-if statements as decpicted in lines 30 to 37 of the notes, because I was dealing with multiple conditions. This resulted in code that was able to successfully generate the correct list when checked using the sandbox. 

`
for (let i = 1; i <= 100; i++) {
   if (i % 3 === 0 && i % 5 === 0){
     console.log("FizzBuzz");
  }
  else if (i % 3 === 0){
    console.log("Fizz")
  }
  else if (i % 5 === 0){
    console.log("Buzz")
  }
  else {
    console.log(i)
  }
  }
`
 
  