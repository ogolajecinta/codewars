# 8kyu

## Counting Sheep

https://www.codewars.com/kata/54edbc7200b811e956000556

Consider an array/list of sheep where some sheep may be missing from their place. We need a function that counts the number of sheep present in the array (true means present).

```JS
function countSheeps(arrayOfSheep) {
  // TODO May the force be with you
  const present = arrayOfSheep.filter( sheeps => sheeps === true);
  return present.length; 
}
```
## Grasshopper - Summation

https://www.codewars.com/kata/55d24f55d7dd296eb9000030

Write a program that finds the summation of every number from 1 to num. The number will always be a positive integer greater than 0.

```JS
var summation = function (num) {
  // Code here
  let sum = 0;
  
  //loop each number
  for (i=1; i <= num; i++)
    sum+= i;
   return sum;
}
```
## Even or Odd

https://www.codewars.com/kata/53da3dbb4a5168369a0000fe

Create a function that takes an integer as an argument and returns "Even" for even numbers or "Odd" for odd numbers.

```JS
function even_or_odd(number) {
  
  //use parseInt() to convert input into integer
  let num = parseInt(number);
  
  if(num%2 == 0 ){
    return ("Even");
  }
  else{
    return ("Odd");
  } 
}

```
## Remove First and Last Character

https://www.codewars.com/kata/56bc28ad5bdaeb48760009b0

It's pretty straightforward. Your goal is to create a function that removes the first and last characters of a string. You're given one parameter, the original string. You don't have to worry with strings with less than two characters.

```JS
function removeChar(str){
 //You got this!
let charRemoved = str.slice(1, str.length-1);

  return charRemoved;
}

```
## Convert a String to a Number

https://www.codewars.com/kata/544675c6f971f7399a000e79

We need a function that can transform a string into a number. What ways of achieving this do you know?

Note: Don't worry, all inputs will be strings, and every string is a perfectly valid representation of an integral number.

```JS
var stringToNumber = function(str){
  // put your code here
  return (parseInt(str));
}

```
## Make UpperCase

https://www.codewars.com/kata/57a0556c7cb1f31ab3000ad7

Write a function which converts the input string to uppercase

```JS
function makeUpperCase(str) {
  // Code here
  return str.toUpperCase();
}
```
