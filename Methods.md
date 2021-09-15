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

