# JavaScript One Liners

<br/>

- Random Number Generator
```JS
const randomNumber = (rangeStart, rangeEnd) => new Date().getTime() % rangeEnd + rangeStart;
```

- String Reverse
```JavaScript
const reverseString = (str) => str.split("").reverse().join("");
```

-  Average of an Array of Number
```JavaScript
const average = (arr) => arr.reduce((a, b) => a + b) / arr.length
``` 
