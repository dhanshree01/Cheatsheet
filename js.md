1. To print something on the console
```js
console.log("hello world");
```
2. Variables are used to store some information
```js
var firstName = "Harshit";
let firstName = "harshit";
```
3. Declare constants
```js
const pi = 3.14;
```
4. String indexing
```js
//  h    a   r   s   h   i   t 
//  0    1   2   3   4   5   6
let firstName = "harshit";
console.log(firstName[0]);              //h
```
5. String properties
```js
console.log(firstName.length);          //7
firstName = firstName.trim();           //Removes whitespaces from both sides of string
firstName = firstName.toUpperCase();    //HARSHIT
firstName = firstName.toLowerCase();    //harshit
let newString = firstName.slice(0,5);   //harshi
```
6. String concatenation
```js
let string1 = "17";
let string2 = "10";
let newString = string1 + string2;
console.log(newString);       //1710
```
7. Data types in JS :-

In JavaScript there are 5 different data types that can contain values:
string, number, boolean, object, function

There are 6 types of objects:
Object, Date, Array, String, Number, Boolean

And 2 data types that cannot contain values:
null, undefined
```js
typeof "John"                 // Returns "string"
typeof 3.14                   // Returns "number"
typeof NaN                    // Returns "number"
typeof false                  // Returns "boolean"
typeof [1,2,3,4]              // Returns "object"
typeof {name:'John', age:34}  // Returns "object"
typeof new Date()             // Returns "object"
typeof function () {}         // Returns "function"
typeof myCar                  // Returns "undefined" *
typeof null                   // Returns "object"
```
8. Type conversions
```js
Number() //converts a variable (or a value) into a number
String() //can convert numbers to strings
```

```js
```
```js
```
