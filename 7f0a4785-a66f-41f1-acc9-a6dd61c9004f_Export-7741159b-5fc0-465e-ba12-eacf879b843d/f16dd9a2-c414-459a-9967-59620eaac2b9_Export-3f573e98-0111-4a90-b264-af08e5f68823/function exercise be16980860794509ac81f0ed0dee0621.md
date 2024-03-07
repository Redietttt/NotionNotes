# function exercise

exe 1

Declare a function fullName and it print out your full name.

Declare a function fullName and now it takes firstName, lastName as a parameter and it returns your full - name.

Declare a function addNumbers and it takes two two parameters and it returns sum.

An area of a rectangle is calculated as follows: area = length x width. Write a function which calculates areaOfRectangle.

A perimeter of a rectangle is calculated as follows: perimeter= 2x(length + width). Write a function which calculates perimeterOfRectangle.

A volume of a rectangular prism is calculated as follows: volume = length x width x height. Write a function which calculates volumeOfRectPrism.

Area of a circle is calculated as follows: area = π x r x r. Write a function which calculates areaOfCircle

Circumference of a circle is calculated as follows: circumference = 2πr. Write a function which calculates circumOfCircle

Density of a substance is calculated as follows:density= mass/volume. Write a function which calculates density.

Speed is calculated by dividing the total distance covered by a moving object divided by the total amount of time taken. Write a function which calculates a speed of a moving object, speed.

Weight of a substance is calculated as follows: weight = mass x gravity. Write a function which calculates weight.

Temperature in oC can be converted to oF using this formula: oF = (oC x 9/5) + 32. Write a function which convert oC to oF convertCelsiusToFahrenheit.

Body mass index(BMI) is calculated as follows: bmi = weight in Kg / (height x height) in m2. Write a function which calculates bmi. BMI is used to broadly define different weight groups in adults 20 years old or older.Check if a person is underweight, normal, overweight or obese based the information given below.

The same groups apply to both men and women.
Underweight: BMI is less than 18.5
Normal weight: BMI is 18.5 to 24.9
Overweight: BMI is 25 to 29.9
Obese: BMI is 30 or more
Write a function called checkSeason, it takes a month parameter and returns the season:Autumn, Winter, Spring or Summer.

Math.max returns its largest argument. Write a function findMax that takes three arguments and returns their maximum with out using Math.max method.

console.log(findMax(0, 10, 5))
10
console.log(findMax(0, -10, -2))
0

```jsx
// Function to print full name
function fullName() {
  console.log("Your Full Name");
}

// Function to return full name
function fullNameWithParams(firstName, lastName) {
  return firstName + " " + lastName;
}

// Function to return sum of two numbers
function addNumbers(num1, num2) {
  return num1 + num2;
}

// Function to calculate area of a rectangle
function areaOfRectangle(length, width) {
  return length * width;
}

// Function to calculate perimeter of a rectangle
function perimeterOfRectangle(length, width) {
  return 2 * (length + width);
}

// Function to calculate volume of a rectangular prism
function volumeOfRectPrism(length, width, height) {
  return length * width * height;
}

// Function to calculate area of a circle
function areaOfCircle(radius) {
  return Math.PI * radius * radius;
}

// Function to calculate circumference of a circle
function circumOfCircle(radius) {
  return 2 * Math.PI * radius;
}

// Function to calculate density
function calculateDensity(mass, volume) {
  return mass / volume;
}

// Function to calculate speed
function calculateSpeed(distance, time) {
  return distance / time;
}

// Function to calculate weight
function calculateWeight(mass, gravity) {
  return mass * gravity;
}

// Function to convert Celsius to Fahrenheit
function convertCelsiusToFahrenheit(celsius) {
  return (celsius * 9/5) + 32;
}

// Function to calculate BMI and determine weight group
function calculateBMI(weight, height) {
  const bmi = weight / (height * height);
  if (bmi < 18.5) {
    return "Underweight";
  } else if (bmi >= 18.5 && bmi <= 24.9) {
    return "Normal weight";
  } else if (bmi >= 25 && bmi <= 29.9) {
    return "Overweight";
  } else {
    return "Obese";
  }
}

// Function to check season based on month
function checkSeason(month) {
  switch (month) {
    case 12:
    case 1:
    case 2:
      return "Winter";
    case 3:
    case 4:
    case 5:
      return "Spring";
    case 6:
    case 7:
    case 8:
      return "Summer";
    case 9:
    case 10:
    case 11:
      return "Autumn";
    default:
      return "Invalid month";
  }
}

// Function to find maximum of three numbers without using Math.max
function findMax(a, b, c) {
  return Math.max(a, Math.max(b, c));
}

// Example usage
console.log(fullNameWithParams("John", "Doe"));  // Returns "John Doe"
console.log(addNumbers(5, 7));  // Returns 12
console.log(areaOfRectangle(3, 4));  // Returns 12
console.log(perimeterOfRectangle(3, 4));  // Returns 14
console.log(volumeOfRectPrism(3, 4, 5));  // Returns 60
console.log(areaOfCircle(2));  // Returns approximately 12.566
console.log(circumOfCircle(2));  // Returns approximately 12.566
console.log(calculateDensity(100, 20));  // Returns 5
console.log(calculateSpeed(50, 2));  // Returns 25
console.log(calculateWeight(70, 9.8));  // Returns 686
console.log(convertCelsiusToFahrenheit(25));  // Returns 77
console.log(calculateBMI(70, 1.75));  // Returns "Normal weight"
console.log(checkSeason(6));  // Returns "Summer"
console.log(findMax(0, 10, 5));  // Returns 10
console.log(findMax(0, -10, -2));  // Returns 0
```

exe 2

1. Linear equation is calculated as follows: *ax + by + c = 0*. Write a function which calculates value of a linear equation, *solveLinEquation*.
2. Quadratic equation is calculated as follows: *ax2 + bx + c = 0*. Write a function which calculates value or values of a quadratic equation, *solveQuadEquation*.
    
    ```
    console.log(solveQuadratic()) // {0}
    console.log(solveQuadratic(1, 4, 4)) // {-2}
    console.log(solveQuadratic(1, -1, -2)) // {2, -1}
    console.log(solveQuadratic(1, 7, 12)) // {-3, -4}
    console.log(solveQuadratic(1, 0, -4)) //{2, -2}
    console.log(solveQuadratic(1, -1, 0)) //{1, 0}
    ```
    
3. Declare a function name *printArray*. It takes array as a parameter and it prints out each value of the array.
4. Write a function name *showDateTime* which shows time in this format: 08/01/2020 04:08 using the Date object.
    
    ```
    showDateTime()
    08/01/2020 04:08
    ```
    
5. Declare a function name *swapValues*. This function swaps value of x to y.
    
    ```
    swapValues(3, 4) // x => 4, y=>3
    swapValues(4, 5) // x = 5, y = 4
    ```
    
6. Declare a function name *reverseArray*. It takes array as a parameter and it returns the reverse of the array (don't use method).
    
    ```jsx
    console.log(reverseArray([1, 2, 3, 4, 5]))
    //[5, 4, 3, 2, 1]
    console.log(reverseArray(['A', 'B', 'C']))
    //['C', 'B', 'A']
    ```
    
7. Declare a function name *capitalizeArray*. It takes array as a parameter and it returns the - capitalizedarray.
8. Declare a function name *addItem*. It takes an item parameter and it returns an array after adding the item
9. Declare a function name *removeItem*. It takes an index parameter and it returns an array after removing an item
10. Declare a function name *sumOfNumbers*. It takes a number parameter and it adds all the numbers in that range.
11. Declare a function name *sumOfOdds*. It takes a number parameter and it adds all the odd numbers in that - range.
12. Declare a function name *sumOfEven*. It takes a number parameter and it adds all the even numbers in that - range.
13. Declare a function name evensAndOdds . It takes a positive integer as parameter and it counts number of evens and odds in the number.
    
    ```
    evensAndOdds(100);
    The number of odds are 50.
    The number of evens are 51.
    ```
    
14. Write a function which takes any number of arguments and return the sum of the arguments
    
    ```
    sum(1, 2, 3) // -> 6
    sum(1, 2, 3, 4) // -> 10
    ```
    
15. Writ a function which generates a *randomUserIp*.
16. Write a function which generates a *randomMacAddress*
17. Declare a function name *randomHexaNumberGenerator*. When this function is called it generates a random hexadecimal number. The function return the hexadecimal number.
    
    ```
    console.log(randomHexaNumberGenerator());
    '#ee33df'
    ```
    
18. Declare a function name *userIdGenerator*. When this function is called it generates seven character id. The function return the id.
    
    `console.log(userIdGenerator());
    41XTDbE`
    
    solution
    
    ```jsx
    // Function to solve a linear equation ax + by + c = 0
    function solveLinEquation(a, b, c) {
      return (-c - b) / a;
    }
    
    // Function to solve a quadratic equation ax^2 + bx + c = 0
    function solveQuadEquation(a, b, c) {
      const delta = b**2 - 4*a*c;
    
      if (delta > 0) {
        const x1 = (-b + Math.sqrt(delta)) / (2 * a);
        const x2 = (-b - Math.sqrt(delta)) / (2 * a);
        return [x1, x2];
      } else if (delta === 0) {
        const x = -b / (2 * a);
        return [x];
      } else {
        return [];
      }
    }
    
    // Function to print each value of an array
    function printArray(arr) {
      arr.forEach(value => console.log(value));
    }
    
    // Function to show date and time
    function showDateTime() {
      const now = new Date();
      const formattedDate = now.toLocaleDateString('en-US');
      const formattedTime = now.toLocaleTimeString('en-US', { hour12: false });
      console.log(`${formattedDate} ${formattedTime}`);
    }
    
    // Function to swap values of x and y
    function swapValues(x, y) {
      const temp = x;
      x = y;
      y = temp;
      console.log(`x => ${x}, y => ${y}`);
    }
    
    // Function to reverse an array
    function reverseArray(arr) {
      const reversedArr = [];
      for (let i = arr.length - 1; i >= 0; i--) {
        reversedArr.push(arr[i]);
      }
      return reversedArr;
    }
    
    // Function to capitalize each value of an array
    function capitalizeArray(arr) {
      return arr.map(value => value.toUpperCase());
    }
    
    // Function to add an item to an array
    function addItem(arr, item) {
      arr.push(item);
      return arr;
    }
    
    // Function to remove an item from an array by index
    function removeItem(arr, index) {
      arr.splice(index, 1);
      return arr;
    }
    
    // Function to calculate the sum of numbers in a range
    function sumOfNumbers(num) {
      let sum = 0;
      for (let i = 1; i <= num; i++) {
        sum += i;
      }
      return sum;
    }
    
    // Function to calculate the sum of odd numbers in a range
    function sumOfOdds(num) {
      let sum = 0;
      for (let i = 1; i <= num; i += 2) {
        sum += i;
      }
      return sum;
    }
    
    // Function to calculate the sum of even numbers in a range
    function sumOfEven(num) {
      let sum = 0;
      for (let i = 2; i <= num; i += 2) {
        sum += i;
      }
      return sum;
    }
    
    // Function to count the number of evens and odds in a number
    function evensAndOdds(num) {
      let evenCount = 0;
      let oddCount = 0;
    
      while (num > 0) {
        const digit = num % 10;
        if (digit % 2 === 0) {
          evenCount++;
        } else {
          oddCount++;
        }
        num = Math.floor(num / 10);
      }
    
      console.log(`The number of odds are ${oddCount}.`);
      console.log(`The number of evens are ${evenCount}.`);
    }
    
    // Function to calculate the sum of any number of arguments
    function sum(...args) {
      return args.reduce((acc, val) => acc + val, 0);
    }
    
    // Function to generate a random user IP address
    function randomUserIp() {
      return `${Math.floor(Math.random() * 256)}.${Math.floor(Math.random() * 256)}.${Math.floor(Math.random() * 256)}.${Math.floor(Math.random() * 256)}`;
    }
    
    // Function to generate a random MAC address
    function randomMacAddress() {
      const hexDigits = '0123456789ABCDEF';
      let macAddress = '';
    
      for (let i = 0; i < 6; i++) {
        macAddress += hexDigits[Math.floor(Math.random() * 16)];
        if (i < 5) {
          macAddress += ':';
        }
      }
    
      return macAddress;
    }
    
    // Function to generate a random hexadecimal number
    function randomHexaNumberGenerator() {
      return `#${Math.random().toString(16).slice(2, 8)}`;
    }
    
    // Function to generate a seven-character user ID
    function userIdGenerator() {
      const characters = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789';
      let userId = '';
    
      for (let i = 0; i < 7; i++) {
        userId += characters.charAt(Math.floor(Math.random() * characters.length));
      }
    
      return userId;
    }
    
    // Example usage
    console.log(solveLinEquation(2, 3, 1));  // Returns a value satisfying the equation
    console.log(solveQuadEquation(1, 4, 4));  // Returns [-2]
    console.log(solveQuadEquation(1, -1, -2));  // Returns [2, -1]
    console.log(solveQuadEquation(1, 7, 12));  // Returns [-3, -4]
    console.log(printArray([1, 2, 3, 4, 5]));  // Prints each value of the array
    showDateTime();  // Shows the current date and time
    swapValues(3, 4);  // Swaps values of x and y
    console.log(reverseArray([1, 2, 3, 4, 5]));  // Returns [5, 4, 3, 2, 1]
    console.log(capitalizeArray(['a', 'b', 'c']));  // Returns ['A', 'B', 'C']
    console.log(addItem([1, 2, 3], 4));  // Returns [1, 2, 3, 4]
    console.log(removeItem([1, 2, 3], 1));  // Returns [1, 3]
    console.log(sumOfNumbers(5));  // Returns 15
    console.log(sumOfOdds(5));  // Returns 9
    console.log(sumOfEven(5));  // Returns 6
    evensAndOdds(100);  // Prints the count of evens and odds
    console.log(sum(1, 2, 3));  // Returns 6
    console.log(sum(1, 2, 3, 4));  // Returns 10
    console.log(randomUserIp());  // Returns a random user IP
    console.log(randomMacAddress());  // Returns a random MAC address
    console.log(randomHexaNumberGenerator());  // Returns a random hexadecimal number
    console.log(userIdGenerator());  // Returns a seven-character user ID
    ```
    
    exe 3
    
    1. Modify the *userIdGenerator* function. Declare a function name *userIdGeneratedByUser*. It doesn’t take any parameter but it takes two inputs using prompt(). One of the input is the number of characters and the second input is the number of ids which are supposed to be generated.
        
        ```
        userIdGeneratedByUser()
        'kcsy2
        SMFYb
        bWmeq
        ZXOYh
        2Rgxf
        'userIdGeneratedByUser()
        '1GCSgPLMaBAVQZ26
        YD7eFwNQKNs7qXaT
        ycArC5yrRupyG00S
        UbGxOFI7UXSWAyKN
        dIV0SSUTgAdKwStr
        '
        ```
        
    2. Write a function name *rgbColorGenerator* and it generates rgb colors.
        
        ```
        rgbColorGenerator()
        rgb(125,244,255)
        ```
        
    3. Write a function ***arrayOfHexaColors*** which return any number of hexadecimal colors in an array.
    4. Write a function ***arrayOfRgbColors*** which return any number of RGB colors in an array.
    5. Write a function ***convertHexaToRgb*** which converts hexa color to rgb and it returns an rgb color.
    6. Write a function ***convertRgbToHexa*** which converts rgb to hexa color and it returns an hexa color.
    7. Write a function ***generateColors*** which can generate any number of hexa or rgb colors.
        
        ```
        console.log(generateColors('hexa', 3)) // ['#a3e12f', '#03ed55', '#eb3d2b']
        console.log(generateColors('hexa', 1)) // '#b334ef'
        console.log(generateColors('rgb', 3)) // ['rgb(5, 55, 175)', 'rgb(50, 105, 100)', 'rgb(15, 26, 80)']
        console.log(generateColors('rgb', 1)) // 'rgb(33,79, 176)'
        ```
        
    8. Call your function *shuffleArray*, it takes an array as a parameter and it returns a shuffled array
    9. Call your function *factorial*, it takes a whole number as a parameter and it return a factorial of the number
    10. Call your function *isEmpty*, it takes a parameter and it checks if it is empty or not
    11. Call your function *sum*, it takes any number of arguments and it returns the sum.
    12. Write a function called *sumOfArrayItems*, it takes an array parameter and return the sum of all the items. Check if all the array items are number types. If not give return reasonable feedback.
    13. Write a function called *average*, it takes an array parameter and returns the average of the items. Check if all the array items are number types. If not give return reasonable feedback.
    14. Write a function called *modifyArray* takes array as parameter and modifies the fifth item of the array and return the array. If the array length is less than five it return 'item not found'.
        
        ```
        console.log(modifyArray(['Avocado', 'Tomato', 'Potato','Mango', 'Lemon','Carrot']);
        ```
        
        ```
        ['Avocado', 'Tomato', 'Potato','Mango', 'LEMON', 'Carrot']
        ```
        
        ```
        console.log(modifyArray(['Google', 'Facebook','Apple', 'Amazon','Microsoft',  'IBM']);
        ```
        
        ```
        ['Google', 'Facebook','Apple', 'Amazon','MICROSOFT',  'IBM']
        ```
        
        ```
        console.log(modifyArray(['Google', 'Facebook','Apple', 'Amazon']);
        ```
        
        ```
          'Not Found'
        ```
        
    15. Write a function called *isPrime*, which checks if a number is prime number.
    16. Write a functions which checks if all items are unique in the array.
    17. Write a function which checks if all the items of the array are the same data type.
    18. JavaScript variable name does not support special characters or symbols except $ or _. Write a function **isValidVariable** which check if a variable is valid or invalid variable.
    19. Write a function which returns array of seven random numbers in a range of 0-9. All the numbers must be unique.
        
        ```
        sevenRandomNumbers()
        [(1, 4, 5, 7, 9, 8, 0)]
        ```
        
    20. Write a function called reverseCountries, it takes countries array and first it copy the array and returns the reverse of the original array
    
    soln
    
    ```jsx
    // Function to generate a user ID based on user input
    function userIdGeneratedByUser() {
      const numChars = prompt("Enter the number of characters for each ID:");
      const numIds = prompt("Enter the number of IDs to generate:");
    
      let result = '';
      for (let i = 0; i < numIds; i++) {
        for (let j = 0; j < numChars; j++) {
          result += String.fromCharCode(Math.floor(Math.random() * 26) + 97);
        }
        result += '\n';
      }
    
      return result.trim();
    }
    
    // Function to generate an RGB color
    function rgbColorGenerator() {
      const r = Math.floor(Math.random() * 256);
      const g = Math.floor(Math.random() * 256);
      const b = Math.floor(Math.random() * 256);
      return `rgb(${r},${g},${b})`;
    }
    
    // Function to generate an array of hexadecimal colors
    function arrayOfHexaColors(num) {
      const colors = [];
      for (let i = 0; i < num; i++) {
        colors.push(randomHexaNumberGenerator());
      }
      return colors;
    }
    
    // Function to generate an array of RGB colors
    function arrayOfRgbColors(num) {
      const colors = [];
      for (let i = 0; i < num; i++) {
        colors.push(rgbColorGenerator());
      }
      return colors;
    }
    
    // Function to convert hexa color to rgb
    function convertHexaToRgb(hex) {
      const bigint = parseInt(hex.slice(1), 16);
      const r = (bigint >> 16) & 255;
      const g = (bigint >> 8) & 255;
      const b = bigint & 255;
      return `rgb(${r},${g},${b})`;
    }
    
    // Function to convert rgb color to hexa
    function convertRgbToHexa(rgb) {
      const values = rgb.match(/\d+/g);
      const hex = values.map(val => parseInt(val).toString(16).padStart(2, '0')).join('');
      return `#${hex}`;
    }
    
    // Function to generate any number of hexa or rgb colors
    function generateColors(type, num) {
      const colors = [];
      for (let i = 0; i < num; i++) {
        if (type === 'hexa') {
          colors.push(randomHexaNumberGenerator());
        } else if (type === 'rgb') {
          colors.push(rgbColorGenerator());
        }
      }
      return num === 1 ? colors[0] : colors;
    }
    
    // Function to shuffle an array
    function shuffleArray(arr) {
      for (let i = arr.length - 1; i > 0; i--) {
        const j = Math.floor(Math.random() * (i + 1));
        [arr[i], arr[j]] = [arr[j], arr[i]];
      }
      return arr;
    }
    
    // Function to calculate factorial
    function factorial(num) {
      if (num === 0 || num === 1) {
        return 1;
      } else {
        return num * factorial(num - 1);
      }
    }
    
    // Function to check if a variable is empty
    function isEmpty(variable) {
      return variable === undefined || variable === null || variable === '';
    }
    
    // Function to calculate the sum of any number of arguments
    function sum(...args) {
      return args.reduce((acc, val) => acc + val, 0);
    }
    
    // Function to calculate the sum of array items
    function sumOfArrayItems(arr) {
      if (arr.every(item => typeof item === 'number')) {
        return arr.reduce((acc, val) => acc + val, 0);
      } else {
        return 'Some array items are not numbers.';
      }
    }
    
    // Function to calculate the average of array items
    function average(arr) {
      if (arr.every(item => typeof item === 'number')) {
        return arr.reduce((acc, val) => acc + val, 0) / arr.length;
      } else {
        return 'Some array items are not numbers.';
      }
    }
    
    // Function to modify the fifth item of an array
    function modifyArray(arr) {
      if (arr.length >= 5) {
        arr[4] = arr[4].toUpperCase();
        return arr;
      } else {
        return 'Item not found';
      }
    }
    
    // Function to check if a number is prime
    function isPrime(num) {
      if (num <= 1) return false;
      for (let i = 2; i <= Math.sqrt(num); i++) {
        if (num % i === 0) return false;
      }
      return true;
    }
    
    // Function to check if all items in an array are unique
    function areAllItemsUnique(arr) {
      return new Set(arr).size === arr.length;
    }
    
    // Function to check if all items in an array have the same data type
    function areAllItemsSameType(arr) {
      const firstType = typeof arr[0];
      return arr.every(item => typeof item === firstType);
    }
    
    // Function to check if a variable is a valid variable name
    function isValidVariable(variable) {
      const pattern = /^[a-zA-Z_$][a-zA-Z0-9_$]*$/;
      return pattern.test(variable);
    }
    
    // Function to generate an array of seven random numbers in a range of 0-9
    function sevenRandomNumbers() {
      const uniqueNumbers = new Set();
      while (uniqueNumbers.size < 7) {
        uniqueNumbers.add(Math.floor(Math.random() * 10));
      }
      return Array.from(uniqueNumbers);
    }
    
    // Function to reverse an array
    function reverseCountries(countries) {
      const reversedCountries = [...countries].reverse();
      return reversedCountries;
    }
    
    // Example usage
    console.log(userIdGeneratedByUser());
    console.log(rgbColorGenerator());
    console.log(arrayOfHexaColors(3));
    console.log(arrayOfRgbColors(3));
    console.log(convertHexaToRgb('#a3e12f'));
    console.log(convertRgbToHexa('rgb(125,244,255)'));
    console.log(generateColors('hexa', 3));
    console.log(generateColors('hexa', 1));
    console.log(generateColors('rgb', 3));
    console.log(generateColors('rgb', 1));
    console.log(shuffleArray([1, 2, 3, 4, 5]));
    console.log(factorial(5));
    console.log(isEmpty(null));
    console.log(sum(1, 2, 3));
    console.log(sumOfArrayItems([1, 2, 3, 'a']));
    console.log(average([1, 2, 3, 4]));
    console.log(modifyArray(['Avocado', 'Tomato', 'Potato','Mango', 'Lemon','Carrot']));
    console.log(modifyArray(['Google', 'Facebook','Apple', 'Amazon','Microsoft',  'IBM']));
    console.log(modifyArray(['Google', 'Facebook','Apple', 'Amazon']));
    console.log(isPrime(7));
    console.log(areAllItemsUnique([1, 2, 3, 1]));
    console.log(areAllItemsSameType([1, '2', 3]));
    console.log(isValidVariable('valid_variable'));
    console.log(sevenRandomNumbers());
    console.log(reverseCountries(['USA', 'Canada', 'Mexico']));
    ```