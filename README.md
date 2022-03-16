<h1 align="center"> 

JavaScript One Liners 

</h1>

<br><h2 align="center"> ARRAY </h2>

### Average of an Array of Number

```JavaScript
const average = (arr) => arr.reduce((a, b) => a + b) / arr.length;
```

### Sort an Array

```JavaScript
const sort = (arr) => arr.slice().sort((a, b) => a - b);
```

### Clone an Array

```JavaScript
const clone = (arr) => arr.slice();
```

```JavaScript
const clone = (arr) => [...arr];
```

### Find Unique Values in an Array

```JavaScript
const findUniqueValues = (arr) => arr.filter((i) => arr.indexOf(i) === arr.lastIndexOf(i));
```

### Get the Last Element from an Array

```JavaScript
const lastElement = (arr) => arr.slice(-1)[0];
```

```JavaScript
const lastElement = (arr) => arr.slice().pop();
```


### Shuffle an Array

```JavaScript
const shuffle = (arr) => arr.slice().sort(() => Math.random() - 0.5);
```

### Remove Duplicates from an Array

```JavaScript
const removeDuplicates = (arr) => [...new Set(arr)];
```

### Merge two Arrays

```JavaScript
const merge = (arr1, arr2) => [].concat(arr1, arr2);
```

```JavaScript
const merge = (arr1, arr2) => [...arr1, ...arr2];
```

### Merge and Remove the Duplications

```JavaScript
const merge = (arr1, arr2) => [...new Set(arr1.concat(arr2))];
```

```JavaScript
const merge = (arr1, arr2) => [...new Set([...arr1, ...arr2])];
```

### Remove Falsy value from Array

```JavaScript
const removeFalsyValues = (arr) => arr.filter(x => x);
```

```JavaScript
const removeFalsyValues = (arr) => arr.filter(Boolean);
```

<br><h2 align="center"> RANDOM </h2>

### Random Number Generator

```JavaScript
const randomNumber = (rangeStart, rangeEnd) => new Date().getTime() % rangeEnd + rangeStart;
```

```JavaScript
const randomNumber = (min, max) => Math.floor(Math.random() * (max - min + 1) + min);
```

### Random Hexadecimal Color Generator

```JavaScript
const randomHexColor = () => `#${Math.random().toString(16).slice(2, 8).padEnd(6, '0')}`;
```

### Random Boolean Generator
```JavaScript
const randomBoolean = () => Math.random() >= 0.5;
```

<br><h2 align="center"> STRING </h2>

### Capitalize a String

```JavaScript
const capitalize = (str) => str.charAt(0).toUpperCase() + str.slice(1);
```

### String Reverse

```JavaScript
const reverseString = (str) => str.split("").reverse().join("");
```

```JavaScript
const reverseString = (str) => [...str].reverse().join();
```

### Convert a String to a Number

```JavaScript
const toNumber = (str) => Number(str);
```

```JavaScript
const toNumber = (str) => +str;
```

### Convert a String to a Character Array

```JavaScript
const toCharArray = (str) => str.split('');
```

### Convert Snake case to Camel case

```JavaScript
const snakeToCamel = (str) => str.toLowerCase().replace(/(_\w)/g, (word) => word.toUpperCase().substr(1));
```

<br><h2 align="center"> DATE </h2>

### Days between two dates

```JavaScript
const daysBetweenDates = (date1, date2) => Math.ceil(Math.abs(date1 - date2) / (1000 * 60 * 60 * 24));
```

### Weekday of a Date

```JavaScript
const getWeekday = (date) => ['Sunday','Monday','Tuesday','Wednesday','Thursday','Friday','Saturday'][date.getDay()];
```

```JavaScript
const getWeekday = (date) => date.toLocaleString('en-US', {weekday: 'long'});
```

<br><h2 align="center"> VALIDATION </h2>

### Check if an Array Is Empty

```JavaScript
const isEmpty = (arr) => !Array.isArray(arr) || !arr.length;
```

### Check if Array includes a Value

```JavaScript
const includes = (arr, value) => arr.indexOf(value) != -1;
```

```JavaScript
const includes = (arr, value) => arr.includes(value);
```

### Check if the date is Weekend

```JavaScript
const isWeekend = (date) => [5, 6].indexOf(date.getDay()) !== -1;
```

<br><h2 align="center"> MISCELLANEOUS </h2>

### Get selected text

```JavaScript
const getSelectedText = () => window.getSelection().toString();
```
### Toggle a Boolean

```JavaScript
const toggle = (flag) => !flag;
```



<br><h1 align="center"> 

Reference 

</h1>

* https://medium.com/dailyjs/10-javascript-oneliners-you-have-got-to-add-your-arsenal-as-a-developer-b733cbb973b2
* https://dev.to/saviomartin/20-killer-javascript-one-liners-94f
* https://www.makeuseof.com/javascript-one-liners-you-should-know/
* https://www.samanthaming.com/tidbits/?filter=JS#CodeTidbits
* https://dev.to/ruppysuppy/7-killer-one-liners-in-javascript-one
