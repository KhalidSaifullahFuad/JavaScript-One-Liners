# JavaScript One Liners

<br/>

- Random Number Generator

```JavaScript
const randomNumber = (rangeStart, rangeEnd) => new Date().getTime() % rangeEnd + rangeStart;
```

- String Reverse

```JavaScript
const reverseString = (str) => str.split("").reverse().join("");
```

- Average of an Array of Number

```JavaScript
const average = (arr) => arr.reduce((a, b) => a + b) / arr.length;
```

- Capitalize a String

```JavaScript
const capitalize = (str) => str.charAt(0).toUpperCase() + str.slice(1);
```

- Days between two dates

```JavaScript
const daysBetweenDates = (date1, date2) => Math.abs(date1.getTime() - new date2.getTime()) / (1000 * 3600 * 24);
```
