# JavaScript One Liners

<!-- 
https://medium.com/dailyjs/10-javascript-oneliners-you-have-got-to-add-your-arsenal-as-a-developer-b733cbb973b2
https://dev.to/saviomartin/20-killer-javascript-one-liners-94f
https://www.makeuseof.com/javascript-one-liners-you-should-know/
-->

<!--------- RANDOM STUFF -------->

### Random Number Generator

```JavaScript
const randomNumber = (rangeStart, rangeEnd) => new Date().getTime() % rangeEnd + rangeStart;
```

```JavaScript
const randomNumber = (min, max) => Math.floor(Math.random() * (max - min + 1) + min);
```

### Random Hexadecimal Color Generator

```JavaScript
const randomHexColor = () => `#${Math.floor(Math.random()*0xFFFFFF).toString(16).padStart(6,'0')}`;
```

<!------------ STRING ----------->

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

### Convert Snake case to Camel case

```JavaScript
const snakeToCamel = (str) => str.toLowerCase().replace(/(_\w)/g, (word) => word.toUpperCase().substr(1));
```

<!------------ ARRAY ----------->

### Check if an Array Is Empty

```JavaScript
const isEmpty = (arr) => !Array.isArray(arr) || !arr.length;
```

### Average of an Array of Number

```JavaScript
const average = (arr) => arr.reduce((a, b) => a + b) / arr.length;
```

### Find Unique Values in an Array

```JavaScript
const findUniqueValues = (arr) => arr.filter((i) => arr.indexOf(i) === arr.lastIndexOf(i));
```

### Remove Duplicates from an Array

```JavaScript
const removeDuplicates = (arr) => [...new Set(arr)];
```

### Shuffle an Array

```JavaScript
const shuffle = (arr) => arr.slice().sort(() => Math.random() - 0.5);
```

### Remove Falsy value from Array

```JavaScript
const removeFalsyValues = (arr) => arr.filter(x=>x)
```

```JavaScript
const removeFalsyValues = (arr) => arr.filter(Boolean)
```

<!------------- DATE ------------>

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

### Check if the date is Weekend

```JavaScript
const isWeekend = (date) => [5, 6].indexOf(date.getDay()) !== -1;
```
