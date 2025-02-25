# FtoC Documentation
In order to write a program that converts 99 Fahrenheit to Celsius, I started by creating a binding, or in other words, assigning the variable f with the value 99 using the keyword const. This is demonstarted in the [Program Structure chapter of Eloquent JavaScrpt by Marijn Haverbeke](https://eloquentjavascript.net/02_program_structure.html). After creating a binding for the variable f to represent Fahrenheit using the keyword const and an equal sign, I then created another binding for the variable c for Celsius. Rather than assigning a value to c, I assigned the equation that converts Fahrenheit to Celsius, and I used the constant f in this equation since I had previously assigned f to 99. I made sure to use parenthesis to group expressions together to establish the order in which the operations should be performed. I referred to the [Values, Types, And Operators chpater of the Eloquent JavaScript textbook](https://eloquentjavascript.net/01_values.html) to format this correctly with the proper operator symbols. My last line of code simply instructed to calculate for c as depicted in the aforementioned chapter of Eloquent JavaScript as well as the Bindings (Variables) section of the notes in the repository [261sp25](https://github.com/rdwrome/261sp25/blob/main/03Operators%26Bindings/codealong.js). 

`
const f = 99;
const c = ((f - 32) * 5/9);
console.log(c);
`

