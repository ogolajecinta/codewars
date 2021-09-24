# 7kyu

## Jaden Case String

https://www.codewars.com/kata/5390bac347d09b7da40006f6

Your task is to convert strings to how they would be written by Jaden Smith. The strings are actual quotes from Jaden Smith, but they are not capitalized in the same way he originally typed them.

```JS
String.prototype.toJadenCase = function () {
  //...
  var str = "";
  var words = this.split(' ');
  
  for(let i=0; i< words.length; i++ ){
    words[i] = words[i][0].toUpperCase() + words[i].substr(1);
  }
  return words.join(' ');
}; 
```
Alternatively:
```JS
String.prototype.toJadenCase = function () {
  var newStr = "";
  
  this.split(" ").forEach(function(s) { 
      newStr = newStr + " " + s.substring(0,1).toUpperCase() + s.substring(1); 
  });

  return newStr.substr(1);
};
```
## Odd or Even?

https://www.codewars.com/kata/5949481f86420f59480000e7

Given a list of integers, determine whether the sum of its elements is odd or even.

Give your answer as a string matching "odd" or "even".

If the input array is empty consider it as: [0] (array with a zero).

```JS
function oddOrEven(array) {
   //enter code here
   
  return (array.reduce((a, b) => a + b, 0) % 2 === 0)? 'even' : 'odd';

}
```