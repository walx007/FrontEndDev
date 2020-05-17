#### Object Literal Shorthand  
A recurring trend in ES6 is to remove unnecessary repetition in your code. By removing unnecessary repetition, your code becomes easier to read and more concise.
This trend continues with the introduction of new shorthand ways for initializing objects and adding methods to objects

##### Object literal shorthand
- If object properties have the same name as the variables being assigned to them, then you can drop the duplicate variable names.

` let type = 'quartz';
let color = 'rose';
let carat = 21.29;

const gemstone = {
  type: type,
  color: color,
  carat: carat
};

console.log(gemstone); `

this can be writtrn as -

`let type = 'quartz';
let color = 'rose';
let carat = 21.29;

const gemstone = { type, color, carat};`


#### Shorthand method names  
In this example, an anonymous function is being assigned to the property calculateWorth, but is the function keyword really needed?
In ES6, it’s not!
-In this example, an anonymous function is being assigned to the property calculateWorth, but is the function keyword really needed? In ES6, it’s not! 

let type = 'quartz';
let color = 'rose';
let carat = 21.29;

`const gemstone = {
  type,
  color,
  carat,
  calculateWorth: function() {
    // will calculate worth of gemstone based on type, color, and carat
  }
};`

In above code we can drop function() keyword;
> Since you only need to reference the gemstone’s calculateWorth property in order to call the function, having the function keyword is redundant, so it can be dropped.

 


