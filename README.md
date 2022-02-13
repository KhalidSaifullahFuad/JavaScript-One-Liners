# JavaScript One Liners

<br/>

<!------------ NUMBER ----------->

- Random Number Generator

```JavaScript
const randomNumber = (rangeStart, rangeEnd) => new Date().getTime() % rangeEnd + rangeStart;
```

<!------------ STRING ----------->

- Capitalize a String

```JavaScript
const capitalize = (str) => str.charAt(0).toUpperCase() + str.slice(1);
```

- String Reverse

```JavaScript
const reverseString = (str) => str.split("").reverse().join("");
```

<!------------ ARRAY ----------->

- Average of an Array of Number

```JavaScript
const average = (arr) => arr.reduce((a, b) => a + b) / arr.length;
```

- Remove Duplicates from an Array

```JavaScript
const removeDuplicates = (arr) => [...new Set(arr)];
```

- Shuffle an Array

```JavaScript
const shuffle = (arr) => arr.slice().sort(() => Math.random() - 0.5);
```

<!------------- DATE ------------>

- Days between two dates

```JavaScript
const daysBetweenDates = (date1, date2) => Math.abs(date1.getTime() - new date2.getTime()) / (1000 * 3600 * 24);
```
