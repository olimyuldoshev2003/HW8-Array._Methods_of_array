# HW8-Array.\_Methods_of_array

# Array in JS

## What's array in JS?

An <span style="color:red;">array</span>is an object that holds values (of any type) not particularly in named properties/keys,
but rather in numerically indexed position
In JavaScript, an array is an ordered list of values. Each value is called an element specified by
an index. ... First, an array can hold values of mixed types.

**An array is a special variable, which can hold more than one value:**

### Creating an array

1. Using an array literal:

<h2 style="color:red;">Syntax:</h2>

```js
const arr_name = [item1, item2, ..., item n];
```

<h2 style="color:red;">Example:</h2>

```js
const arr = [1, 2, "three", true];
console.log(arr[3]);
```

<h2 style="color:red;">Output:</h2>

```js
true;
```

2. Using the new keyword:

<h2 style="color:red;">Syntax:</h2>

```js
const arr_name = new Array(item1, item2, ..., item n);
```

<h2 style="color:red;">Example:</h2>

```js
const arr = new Array(1, 2, "three", true);
console.log(arr[3]);
```

<h2 style="color:red;">Output:</h2>

```js
true;
```

**Notice:** How you saw array in js can accept the different data types of values. So that's why when you use array in js, look up that which type of data type you're using in array.

## CHANGE ELEMENTS IN ARRAY

You can also <span style="color:red;">add elements</span> or change the elements by accessing the index value
Suppose, an array has two elements. If you try to add an element at index 3 (fourth
element), the third element will be <span style="color:red;">undefined</span>.

<h2 style="color:red;">Example:</h2>

```js
let arr = [1, 2, 3, 4, 5];
arr[4] = 10;
console.log(arr);
```

<h2 style="color:red;">Output:</h2>

```js
[1, 2, 3, 4, 10];
```

## ARRAY METHODS

In JS we have many types of methods of array like methods of string, but the main array methods are these:

> pop()

> join()

> indexOf()

> concat()

> shift()

> includes()

> toString()

> push()

> splice()

> slice()

> toReversed()

### Callback methods (methods, which accept the function in their parameters):

> forEach()

> map()

> find()

> filter()

> reduce()

> toSorted()

## Array Method push()

The push() method adds one or more elements to the end of an array and returns the
new length of the array.
The element(s) to add to the end of the array.

<h2 style="color:red;">Syntax:</h2>

```js
push(element0, element1, /* … ,*/ elementN);
```

<h2 style="color:red;">Example 1:</h2>

```js
let arr = [1, 2, 3, 4, 5];
arr.push(6);
console.log(arr);
```

<h2 style="color:red;">Output:</h2>

```js
[1, 2, 3, 4, 5, 6];
```

<h2 style="color:red;">Example 2:</h2>

```js
let arr = [1, 2, 3, 4, 5];
let count = arr.push(10);
console.log(count);
```

<h2 style="color:red;">Output:</h2>

```js
6;
```

## Array Method pop()

The pop() method removes the last element from an array and returns that element.
This method changes the length of the array.

<h2 style="color:red;">Syntax:</h2>

```js
pop();
```

<h2 style="color:red;">Example:</h2>

```js
let arr = [1, 2, 3, 4, 5];
arr.pop();
console.log(arr);
```

<h2 style="color:red;">Output:</h2>

```js
[1, 2, 3, 4];
```

## Array Method unshift()

The unshift() method adds one or more elements to the beginning of an array and
returns the new length of the array.

<h2 style="color:red;">Syntax:</h2>

```js
unshift(element0, element1, /* … ,*/ elementN);
```

<h2 style="color:red;">Example:</h2>

```js
let arr = [1, 2, 3, 4, 5];
arr.unshift(0);
console.log(arr);
```

<h2 style="color:red;">Output:</h2>

```js
[0, 1, 2, 3, 4, 5];
```

## Array Method shift()

The shift() method removes the first element from an array and returns that removed item. This method changes the length of the array.

<h2 style="color:red;">Syntax:</h2>

```js
pop();
```

<h2 style="color:red;">Example:</h2>

```js
let arr = ["a", "b"];
const poppedValue = arr.shift();
console.log(arr);
```

<h2 style="color:red;">Output:</h2>

```js
["b"];
```

## Array Method toString()

The toString() method returns a string representing the specified array and its
elements.
A string representing the elements of the array.

<h2 style="color:red;">Syntax:</h2>

```js
toString();
```

<h2 style="color:red;">Example:</h2>

```js
let number = [1000, 2000, 3000];
console.log(number.toString());
```

```js
"1000,2000,3000";
```

## Array Method indexOf()

The indexOf() method returns the first index (position) of a specified value. The indexOf() method returns -1 if the value is not found. The indexOf() method starts at a specified index and searches from left to right. By default the search starts at the first element and ends at the last. Negative start values counts from the last element (but still searches from left to right)

<h2 style="color:red;">Syntax:</h2>

```js
array.indexOf(item, start);
```

<h2 style="color:red;">Example:</h2>

```js
const names = ["Florin", "Ivan", "Liam"];
const index = names.indexOf("Ivan");
console.log(index);
```

<h2 style="color:red;">Output:</h2>

```js
1;
```

## Array Method includes()

The includes() method returns true if an array contains a specified value. The includes() method returns false if the value is not found. The includes() method is case sensitive.

<h2 style="color:red;">Syntax:</h2>

```js
array.includes(element, start);
```

<h2 style="color:red;">Example</h2>

```js
const names = ["Florin", "Ivan", "Liam"];
const result = names.includes("Ivan");
console.log(result);
```

<h2 style="color:red;">Output:</h2>

```js
true;
```

## Array Method slice()

The slice() method returns selected elements in an array, as a new array. The slice() method selects from a given start, up to a (not inclusive) given end. The slice() method does not change the original array.

<h2 style="color:red;">Syntax:</h2>

```js
array.slice(start, end);
```

<h2 style="color:red;">Example</h2>

```js
const numbers = [1, 2, 3, 4, 5];
const numbers2 = numbers.slice(3);
console.log(numbers2);
```

<h2 style="color:red;">Output:</h2>

```js
[4, 5];
```

## Array Method concat()

The concat() method concatenates (joins) two or more arrays. The concat() method returns a new array, containing the joined arrays. The concat() method does not change the existing arrays.

<h2 style="color:red;">Syntax:</h2>

```js
array1.concat(array2, array3, ..., arrayX)
```

<h2 style="color:red;">Example</h2>

```js
const a = [1, 2, 3];
const b = [4, 5, 6];
const d = [7, 8, 9];

const c = a.concat(b, d);
console.log(c);
```

<h2 style="color:red;">Output:</h2>

```js
[1, 2, 3, 4, 5, 6, 7, 8, 9];
```

## Array Method splice()

The splice() method adds and/or removes array elements. The splice() method overwrites the original array.
It also changes the length of an array by removing items from it. If you don't specify any.

<h2 style="color:red;">Syntax:</h2>

```js
array.splice(index, howmany, item1, ....., itemX);
```

<h2 style="color:red;">Example 1:</h2>

```js
const numbers = [1, 2, 3, 4, 5];
numbers.splice(2, 3);
console.log(numbers);
```

<h2 style="color:red;">Output:</h2>

```js
[1, 2, 4, 5];
```

<h2 style="color:red;">Example 2:</h2>

```js
const numbers = [1, 2, 3, 4, 5];
numbers.splice(2, 0, 6, 7);
console.log(numbers);
```

<h2 style="color:red;">Output:</h2>

```js
[1, 2, 6, 7, 3, 4, 5];
```

# JS ARRAY METHOD CALLBACK

## Array Method map()

map() creates a new array from calling a function for every array element. map() calls a function once for each element in an array. map() does not execute the function for empty elements. map() does not change the original array.

<h2 style="color:red;">Syntax:</h2>

```js
array.map(function(currentValue, index, arr), thisValue)
```

<h2 style="color:red;">Example:</h2>

```js
const numbers = [1, 2, 3, 4, 5];
const secondNumbers = numbers.map((value, index, array) => {
  return value * 2;
});

console.log(secondNumbers);
```

<h2 style="color:red;">Output:</h2>

```js
[2, 4, 6, 8, 10]
```

## Array Method forEach()

The forEach() method calls a function for each element in an array. The forEach() method is not executed for empty elements.

<h2 style="color:red;">Syntax:</h2>

```js
array.forEach(function(currentValue, index, arr), thisValue)
```

<h2 style="color:red;">Example:</h2>

```js
const arr=[1,2,3,4,5]
arr.forEach((item,index,array)=>{
    console.log(item);
});
```

<h2 style="color:red;">Output:</h2>

```js
1
2
3
4
5
```

## Array Method find()

The find() method returns the value of the first element that passes a test. The find() method executes a function for each array element. The find() method returns undefined if no elements are found. The find() method does not execute the function for empty elements. The find() method does not change the original array.

<h2 style="color:red;">Syntax:</h2>

```js
array.find(function(currentValue, index, arr),thisValue)
```

<h2 style="color:red;">Example:</h2>

```js
const names = ["Florin", "Ivan", "Liam"];
const result = names.find((item) => item === "Ivan");
console.log(result);
```

<h2 style="color:red;">Output:</h2>

```js
Ivan
```

## Array Method reduce()

The reduce() method executes a user-supplied "reducer" callback function on each element
of the array, in order, passing in the return value from the calculation on the preceding
element. The final result of running the reducer across all elements of the array is a single
value.

<h2 style="color:red;">Syntax:</h2>

```js
array.reduce(function(total, currentValue, currentIndex, arr), initialValue)
```

<h2 style="color:red;">Example:</h2>

```js
const numbers=[1,2,3,4,5]
const total = numbers.reduce((accumulator,value,index,arr)=>{
  return  accumulator+value
}, 0)

console.log(total);
```

<h2 style="color:red;">Output:</h2>

```js
15
```

## Array Method filter()

The filter() method creates a shallow copy of a portion of a given array, filtered down to
just the elements from the given array that pass the test implemented by the provided
function. 

<h2 style="color:red;">Syntax:</h2>

```js
array.filter(function(currentValue, index, arr), thisValue)
```

<h2 style="color:red;">Example:</h2>

```js
const array = [1, 2, 3, 4, 5, 6];
const even = array.filter((value) => {
  return value % 2 === 0;
});
console.log(even);
```

<h2 style="color:red;">Output:</h2>

```js
[2, 4, 6]
```

## Array Method toSorted()

The toSorted() method of Array instances is the copying version of the sort() method.
It returns a new array with the elements sorted in ascending order

<h2 style="color:red;">Syntax:</h2>

```js
array.sort(compareFunction)
```

<h2 style="color:red;">Example:</h2>

```js
const numbers=[12,23,345,21,12,11,321,15,97]
let newNumbers = numbers.toSorted((a,b)=>a-b)
console.log(newNumbers);
```

<h2 style="color:red;">Output</h2>

```js
[11, 12, 12, 15, 21, 23, 97, 321, 345]
```

## Method Destructuring

The destructuring assignment syntax is a JavaScript expression that makes it
possible to unpack values from arrays, or properties from objects, into distinct
variables.

<h2 style="color:red;">Example:</h2>

```js
let a, b, rest
let arr = [10, 20];
[a, b] = arr;
console.log(a);
console.log(b);
[a, b, ...rest] = [10, 20, 30, 40, 50]
console.log(rest)
```

<h2 style="color:red;">Output</h2>

```js
10
20
[ 30, 40, 50 ]
```

## Method Spread

The spread (...) syntax allows an iterable, such as an array or string, to be
expanded in places where zero or more arguments (for function calls) or
elements (for array literals) are expected. In an object literal, the spread syntax
enumerates the properties of an object and adds the key-value pairs to the object
being created.

<h2 style="color:red;">Example:</h2>

```js
function sum(x, y, z) {
    return x + y + z;
}

const num = [1, 2, 3];
console.log(sum(...num));
```

<h2 style="color:red;">Output</h2>

```js
6
```

## Method Rest

The rest parameter syntax allows a function to accept an indefinite
number of arguments as an array

<h2 style="color:red;">Example</h2>

```js
function sum(...theArgs) {
    return theArgs;
}

console.log(sum(1, 2, 3));
```

<h2 style="color:red;">Output</h2>

```js
[1, 2, 3]
```