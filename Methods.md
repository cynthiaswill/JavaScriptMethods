# JavaScript Methods
This reference sheet has been created to provide a quick and easy lookup for various built-in JavaScript methods. This list will be primarily written using the arrow syntax (because it's awesome).

## Higher Order Functions [HOFs]
HOFs are functions that accept and/or retrun another function. It's called *higher-order* because instead of operating on strings, numbers, booleans etc it goes higher and operates on functions themselves. But don't think of them as something beyond understanding, *just treat them like premade functions for you to use like any other.*

```
let arr = 10, 20, 15, 5];
let empty = [];
```
#### *.forEach()*
```
const method = arr => {
  arr.forEach(element => empty.push(element))
  return empty
}
```
.foreach() is best used to perform an action on *every* element in the array, such as pushing and pulling. This can replace a for/while loop. Result: empty = [10, 20, 15, 5]

#### *.map()*
```
const method = arr => {
  return arr.map((item) => item * 2);
}
```
.map() is best used to perform a calculation on *every single element* in the array. Result: [20, 40, 30, 10]

#### *.reduce()*
```
const method = arr => {
  return arr.reduce((a, b) => a + b);
}
```
.reduce() is best used to condense an array of numbers into a single number. Result: 50

#### *.filter()*
```
const method = arr => {
  return arr.filter((item) => item < 12);
}
```
.filter() is used to filter an array based on a condition. Result: [10, 5]


## Number Methods

```let decimal = 2.555555;```

```decimal.toFixed(3)```      returns 2.556; <br>
```decimal.toPrecision(5)```  returns 2.5556; <br>
```decimal.toString()```      returns '2.555555' <br>

## String Methods

```let str = 'Testing phrase'```
```str.charAt(0)``` returns 'T'<br>
```str.indexOf('T')``` returns 0<br>
```str.slice(0, 7)``` returns 'Testing' (goes up to but does not include 7, zero index)<br>
```str.slice(-6)``` returns 'phrase' (counts down from the end of the string)<br>
```str.split(" ")``` returns ['Testing', 'phrase']<br>
```str.split("")``` returns ['T','e','s','t','i','n','g','p','h','r','a','s','e']<br>
```str.toLowerCase()``` returns all lowercase string<br>
```str.toUpperCase()``` returns all uppercase string<br>

## Array Methods
```let arr = [1, 2, 3, 4, 5]
let arrTwo = [3, 4]
let arrThree = ['b', 'c', 'a']
let split = str.split("")```

```arr.concat(arrTwo)``` returns [1, 2, 3, 4, 5, 3, 4]<br>
```arr.every(item => item < 3))``` returns  true<br>
```split.join("")``` returns ‘Testing phrase’<br>
```arr.some(item => item > 4)``` returns true<br>
```arr.slice(2, 4)``` returns [3, 4]<br>
```arr.splice(1, 3)``` returns [1, 5] (removes 2, 3, 4 from the array)<br>
```arr.splice(1, 3, 4, 2, 3, 6, 7)``` returns [1, 4, 2, 3, 6, 7, 5] (adds to the array)<br>
```arrThree.sort()``` returns sorted character array<br>
```arrThree.sort(function(a, b){return a - b})``` returns sorted numeric array<br>
```arr.pop()``` removes last element from an array<br>
```arr.push()``` adds last element to an array<br>
```arr.shift()``` removes first element of an array<br>
```arr.unshift()``` adds first element to an array<br>
```let copy = [...arrTwo]``` creates a copy of an array<br>
```let concat = [...arrTwo, ...arrThree]``` concatenates arrays<br>
```let spread = [1, 2, ...arrTwo]``` returns [1, 2, 3, 4]<br>

