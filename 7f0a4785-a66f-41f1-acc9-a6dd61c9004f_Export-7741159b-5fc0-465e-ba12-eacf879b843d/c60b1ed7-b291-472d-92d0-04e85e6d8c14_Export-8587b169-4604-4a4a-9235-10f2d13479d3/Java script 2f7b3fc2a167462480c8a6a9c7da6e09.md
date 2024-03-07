# Java script

```css
console.log('hello world')

firstname ="hanna"
console.log(firstname)

```

data types

```jsx
const x = 5;
const y = "Hello";
```

……… 

- 5 is an integer data.
- "Hello" is a string data.
- **String**: Represents textual data, enclosed in single ('') or double ("") quotes.
- **Number**: Represents numeric data, including integers and floating-point numbers.
- **Boolean**: Represents a logical value, either **`true`** or **`false`**.
- **Undefined**: Represents a variable that has been declared but not assigned a value.
- **Null**: Represents an intentional absence of any object value.
- **Symbol**: Represents unique identifiers, introduced in ECMAScript 6.

string methods 

1. **charAt(index):**
    
    Retrieves the character at a specified index within a string. For instance:
    
    ```jsx
    javascriptCopy code
    var str = "Hello";
    var charAtIndex = str.charAt(1); // charAtIndex will be 'e'
    
    ```
    
2. **concat(str1, str2, ...):**
    
    Combines two or more strings into a single string. Example:
    
    ```jsx
    javascriptCopy code
    var str1 = "Hello";
    var str2 = " World";
    var result = str1.concat(str2); // result will be "Hello World"
    
    ```
    
3. **indexOf(substring):**
    
    Determines the position of the first occurrence of a specified substring within a string:
    
    ```jsx
    javascriptCopy code
    var str = "Hello World";
    var index = str.indexOf("World"); // index will be 6
    
    ```
    
4. **substring(startIndex, endIndex):**
    
    Extracts a portion of a string based on specified start and end indices:
    
    ```jsx
    javascriptCopy code
    var str = "Hello World";
    var substr = str.substring(0, 5); // substr will be "Hello"
    
    ```
    
5. **toUpperCase() / toLowerCase():**
    
    Converts a string to either uppercase or lowercase:
    
    ```jsx
    javascriptCopy code
    var str = "Hello";
    var upper = str.toUpperCase(); // upper will be "HELLO"
    var lower = str.toLowerCase(); // lower will be "hello"
    
    ```
    
6. **replace(oldSubstring, newSubstring):**
    
    Substitutes a specified substring with another substring:
    
    ```jsx
    javascriptCopy code
    var str = "Hello World";
    var newStr = str.replace("World", "Universe"); // newStr will be "Hello Universe"
    
    ```
    
7. **split(separator):**
    
    Divides a string into an array of substrings using a specified separator:
    
    ```jsx
    javascriptCopy code
    var str = "apple,orange,banana";
    var fruits = str.split(","); // fruits will be ["apple", "orange", "banana"]
    
    ```
    
8. **trim():**
    
    Eliminates leading and trailing whitespaces from a string:
    
    ```jsx
    javascriptCopy code
    var str = "   Hello   ";
    var trimmed = str.trim(); // trimmed will be "Hello"
    
    ```
    

# operators

1. **Arithmetic Operators**:
    - **Addition (+)**: Adds two operands.
    - **Subtraction (-)**: Subtracts the right operand from the left operand.
    - **Multiplication (*)**: Multiplies two operands.
    - **Division (/)**: Divides the left operand by the right operand.
    - **Remainder (%)**: Returns the remainder of dividing the left operand by the right operand.
    - **Increment (++)**: Increases the value of an operand by 1.
    - **Decrement (--)**: Decreases the value of an operand by 1.
2. **Assignment Operators**:
    - **Assignment (=)**: Assigns a value to a variable.
    - **Addition Assignment (+=)**: Adds the value of the right operand to the variable and assigns the result to the variable.
    - **Subtraction Assignment (-=)**: Subtracts the value of the right operand from the variable and assigns the result to the variable.
    - **Multiplication Assignment (*=)**: Multiplies the variable by the value of the right operand and assigns the result to the variable.
    - **Division Assignment (/=)**: Divides the variable by the value of the right operand and assigns the result to the variable.
    - **Remainder Assignment (%=)**: Assigns the remainder of dividing the variable by the value of the right operand to the variable.
3. **Comparison Operators**:
    - **Equal to (==)**: Compares two operands for equality.
    - **Not Equal to (!=)**: Compares two operands for inequality.
    - **Strict Equal to (===)**: Compares two operands for equality without type conversion.
    - **Strict Not Equal to (!==)**: Compares two operands for inequality without type conversion.
    - **Greater than (>)**: Checks if the left operand is greater than the right operand.
    - **Less than (<)**: Checks if the left operand is less than the right operand.
    - **Greater than or Equal to (>=)**: Checks if the left operand is greater than or equal to the right operand.
    - **Less than or Equal to (<=)**: Checks if the left operand is less than or equal to the right operand.
4. **Logical Operators**:
    - **Logical AND (&&)**: Returns true if both operands are true.
    - **Logical OR (||)**: Returns true if at least one of the operands is true.
    - **Logical NOT (!)**: Returns the opposite boolean value of the operand.
5. **Unary Operators**:
    - **Unary Plus (+)**: Attempts to convert the operand into a number.
    - **Unary Negation (-)**: Negates the operand.
    - **Logical NOT (!)**: Converts the operand to a boolean value and returns its inverse.
6. **Conditional (Ternary) Operator**:
    - **Conditional (?:)**: Evaluates a condition and returns one of two possible values depending on whether the condition is true or false.
7. **Type Operators**:
    - **typeof**: Returns a string indicating the type of the operand.
    - **instanceof**: Returns true if the specified object is of the specified object type.

```jsx
let x = 5;
let y = 3;

// addition
console.log('x + y = ', x + y);  // 8

// subtraction
console.log('x - y = ', x - y);  // 2

// multiplication
console.log('x * y = ', x * y);  // 15

// division
console.log('x / y = ', x / y);  // 1.6666666666666667

// remainder
console.log('x % y = ', x % y);   // 2

// increment
console.log('++x = ', ++x); // x is now 6
console.log('x++ = ', x++); // prints 6 and then increased to 7
console.log('x = ', x);     // 7

// decrement
console.log('--x = ', --x); // x is now 6
console.log('x-- = ', x--); // prints 6 and then decreased to 5
console.log('x = ', x);     // 5

//exponentiation
console.log('x ** y =', x ** y);
```

```jsx
let salary =50000

let criminalrecord = true

let saving = 100000

let age = 21

let loanApproved =
(age > 18) && (saving > 100000) &&
(criminalrecord || salary >50000 )

console.log(loanApproved)

//if criminal record is false then the output wouldve been true
```

```jsx
conditional 
let age = 11
agestatus =(age>18) ? 'adult' : 'underage'
console.log(agestatus)
```

```jsx
/*
let fullname = 'hanna kebede'
console.log(fullname.split(','))
*/

/*
const arr1 = [23, 4 , 2 , 4 , 328 , 324 , 3 , 5]

let highestvalue = arr1[0]
for (let x = 0; x < arr1.length; x++) {
    highestvalue = (highestvalue < arr1[x]) ?
     arr1[x] : highestvalue
}

*/

/*
for (let x = 0; x < arr1.length; x++) 
{
   // console.log(arr1[x])
    console.log(Math.max(x));
}

*/

/*
.
.
.
.
.
.

let value = ''
for (let index = 0 ; index < 5; index++)
{ 
    value = ''
    for (let index1 = 5 - index ; index1 > 0; index1--){
        value = value + ' * '

    }
  console.log(value)
}

//output
* * * * *
* * * * 
* * * 
* *
*
.
.
.
..
.

*/

/*

//function
let  firstname = 'Hanna'

function greet(name) {

    return 'hello' + name
}
console.info(greet(' hanna'))

// ...... output = hello hanna

*/

/*

function sum( num1 , num2 , num3)
{

    console.log(num1 + num2 + num3)
}

sum(11,23,13)
*/

//arrow function normal function anonymous function
```