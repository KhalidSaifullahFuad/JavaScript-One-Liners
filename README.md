# JavaScript One Liners

<!--------- RANDOM STUFF -------->

### Random Number Generator

```JavaScript
const randomNumber = (rangeStart, rangeEnd) => new Date().getTime() % rangeEnd + rangeStart;
```

### Random Hexadecimal Color

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
// OR
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
// OR
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
// OR
const getWeekday = (date) => date.toLocaleString('en-US', {weekday: 'long'});
```
