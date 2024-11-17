# 100 more easy JS helper functions

| **#** | **Description** | **Function** |
| --- | --- | --- |
| 1. Find the maximum value in an array | `const findMax = arr => Math.max(...arr);` |
| 2. Find the minimum value in an array | `const findMin = arr => Math.min(...arr);` |
| 3. Sum all numbers in an array | `const sumArray = arr => arr.reduce((sum, num) => sum + num, 0);` |
| 4. Get the average of numbers in an array | `const averageArray = arr => arr.reduce((sum, num) => sum + num, 0) / arr.length;` |
| 5. Round a number to the nearest integer | `const roundNumber = num => Math.round(num);` |
| 6. Generate a random number | `const randomNumber = () => Math.random();` |
| 7. Check if a number is even | `const isEven = num => num % 2 === 0;` |
| 8. Check if a number is odd | `const isOdd = num => num % 2 !== 0;` |
| 9. Check if a string is a palindrome | `const isPalindrome = str => str === str.split('').reverse().join('');` |
| 10. Reverse a string | `const reverseString = str => str.split('').reverse().join('');` |
| 11. Count vowels in a string | `const countVowels = str => (str.match(/[aeiou]/gi) || []).length;` |
| 12. Remove whitespace from a string | `const removeWhitespace = str => str.replace(/\s/g, '');` |
| 13. Check if a string contains only letters | `const isAlpha = str => /^[a-zA-Z]+$/.test(str);` |
| 14. Check if a string contains only numbers | `const isNumeric = str => /^[0-9]+$/.test(str);` |
| 15. Replace spaces in a string with dashes | `const replaceSpaces = str => str.replace(/\s+/g, '-');` |
| 16. Capitalize the first letter of a string | `const capitalize = str => str.charAt(0).toUpperCase() + str.slice(1);` |
| 17. Check if an array contains a specific value | `const contains = (arr, value) => arr.includes(value);` |
| 18. Remove duplicates from an array | `const removeDuplicates = arr => [...new Set(arr)];` |
| 19. Flatten a nested array | `const flatten = arr => arr.flat(Infinity);` |
| 20. Find the intersection of two arrays | `const intersection = (arr1, arr2) => arr1.filter(value => arr2.includes(value));` |
| 21. Get the difference between two arrays | `const difference = (arr1, arr2) => arr1.filter(value => !arr2.includes(value));` |
| 22. Check if two arrays are equal | `const arraysEqual = (arr1, arr2) => JSON.stringify(arr1) === JSON.stringify(arr2);` |
| 23. Sort an array of numbers | `const sortNumbers = arr => arr.sort((a, b) => a - b);` |
| 24. Sort an array of strings alphabetically | `const sortStrings = arr => arr.sort();` |
| 25. Remove null or undefined values from an array | `const cleanArray = arr => arr.filter(value => value != null);` |
| 26. Get the unique values from an array of objects | `const uniqueObjects = (arr, key) => [...new Map(arr.map(item => [item[key], item])).values()];` |
| 27. Count the occurrences of each element in an array | `const countOccurrences = arr => arr.reduce((count, item) => (count[item] = (count[item] || 0) + 1, count), {});` |
| 28. Find the most frequent element in an array | `const mostFrequent = arr => Object.entries(countOccurrences(arr)).sort((a, b) => b[1] - a[1])[0][0];` |
| 29. Get the current timestamp | `const getTimestamp = () => Date.now();` |
| 30. Format a date to YYYY-MM-DD | `const formatDate = date => date.toISOString().split('T')[0];` |
| 31. Calculate the difference in days between two dates | `const dateDiffInDays = (date1, date2) => Math.ceil((date2 - date1) / (1000 * 60 * 60 * 24));` |
| 32. Check if a date is in the past | `const isPastDate = date => new Date(date) < new Date();` |
| 33. Check if a date is in the future | `const isFutureDate = date => new Date(date) > new Date();` |
| 34. Add days to a date | `const addDays = (date, days) => new Date(date.setDate(date.getDate() + days));` |
| 35. Check if a year is a leap year | `const isLeapYear = year => (year % 4 === 0 && year % 100 !== 0) || (year % 400 === 0);` |
| 36. Convert seconds to HH:MM:SS format | `const formatTime = seconds => new Date(seconds * 1000).toISOString().substr(11, 8);` |
| 37. Validate a phone number | `const isValidPhoneNumber = phone => /^\+?[0-9]{7,15}$/.test(phone);` |
| 38. Validate a postal code | `const isValidPostalCode = code => /^[0-9]{5}(?:-[0-9]{4})?$/.test(code);` |
| 39. Convert Fahrenheit to Celsius | `const fahrenheitToCelsius = f => (f - 32) * 5 / 9;` |
| 40. Convert Celsius to Fahrenheit | `const celsiusToFahrenheit = c => (c * 9 / 5) + 32;` |
| 41. Check if a value is null or undefined | `const isNullOrUndefined = value => value == null;` |
| 42. Check if a value is an object | `const isObject = value => value !== null && typeof value === 'object';` |
| 43. Check if a value is a string | `const isString = value => typeof value === 'string';` |
| 44. Check if a value is a boolean | `const isBoolean = value => typeof value === 'boolean';` |
| 45. Get the keys of an object | `const getObjectKeys = obj => Object.keys(obj);` |
| 46. Get the values of an object | `const getObjectValues = obj => Object.values(obj);` |
| 47. Get the entries of an object | `const getObjectEntries = obj => Object.entries(obj);` |
| 48. Merge two arrays of objects by a key | `const mergeByKey = (arr1, arr2, key) => arr1.map(item => ({ ...item, ...arr2.find(obj => obj[key] === item[key]) }));` |
| 49. Clone an array | `const cloneArray = arr => [...arr];` |
| 50. Clone an object | `const cloneObject = obj => ({ ...obj });` |
| 51. Convert a string to an array of words | `const stringToWords = str => str.match(/\b(\w+)\b/g);` |
| 52. Convert an array of words to a string | `const wordsToString = arr => arr.join(' ');` |
| 53. Repeat a string n times | `const repeatString = (str, times) => str.repeat(times);` |
| 54. Get the first n elements of an array | `const getFirstElements = (arr, n) => arr.slice(0, n);` |
| 55. Get the last n elements of an array | `const getLastElements = (arr, n) => arr.slice(-n);` |
| 56. Check if a string starts with a specific substring | `const startsWith = (str, substring) => str.startsWith(substring);` |
| 57. Check if a string ends with a specific substring | `const endsWith = (str, substring) => str.endsWith(substring);` |
| 58. Count the number of words in a string | `const countWords = str => str.split(/\s+/).filter(Boolean).length;` |
| 59. Get the unique characters in a string | `const uniqueChars = str => [...new Set(str)];` |
| 60. Convert a number to binary | `const toBinary = num => num.toString(2);` |
| 61. Deep clone an object | `const deepClone = obj => JSON.parse(JSON.stringify(obj));` |
| 62. Convert a string to title case | `const toTitleCase = str => str.replace(/\b\w/g, char => char.toUpperCase());` |
| 63. Get the last element of an array | `const getLastElement = arr => arr[arr.length - 1];` |
| 64. Convert an object to an array of key-value pairs | `const objectToArray = obj => Object.entries(obj);` |
| 65. Check if an object is empty | `const isEmpty = obj => Object.keys(obj).length === 0 && obj.constructor === Object;` |
| 66. Capitalize the first letter of each word in a sentence | `const capitalizeWords = str => str.replace(/\b\w/g, char => char.toUpperCase());` |
| 67. Remove falsy values from an array | `const removeFalsy = arr => arr.filter(Boolean);` |
| 68. Find the longest word in a string | `const longestWord = str => str.split(' ').reduce((longest, current) => current.length > longest.length ? current : longest, '');` |
| 69. Convert an array to a string of comma-separated values | `const arrayToCSV = arr => arr.join(',');` |
| 70. Filter an array of objects by a specific property value | `const filterByProperty = (arr, key, value) => arr.filter(obj => obj[key] === value);` |
| 71. Merge two arrays without duplicates | `const mergeUniqueArrays = (arr1, arr2) => [...new Set([...arr1, ...arr2])];` |
| 72. Generate a random string of a given length | `const generateRandomString = length => Math.random().toString(36).substring(2, 2 + length);` |
| 73. Convert a query string to an object | `const queryStringToObject = str => Object.fromEntries(new URLSearchParams(str));` |
| 74. Convert an object to a query string | `const objectToQueryString = obj => new URLSearchParams(obj).toString();` |
| 75. Check if a string is a valid email | `const isValidEmail = email => /^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(email);` |
| 76. Sort an array of objects by a specific property | `const sortByProperty = (arr, key) => arr.sort((a, b) => a[key] > b[key] ? 1 : -1);` |
| 77. Flatten an array of arrays | `const flattenArray = arr => arr.reduce((flat, current) => flat.concat(current), []);` |
| 78. Check if a value is a number | `const isNumber = value => !isNaN(value);` |
| 79. Format a number to a specific decimal place | `const formatNumber = (num, decimals) => num.toFixed(decimals);` |
| 80. Convert a string to snake_case | `const toSnakeCase = str => str.replace(/\W+/g, '_').toLowerCase();` |
| 81. Convert a string to camelCase | `const toCamelCase = str => str.replace(/_./g, match => match.charAt(1).toUpperCase());` |
| 82. Find the unique elements in an array | `const uniqueElements = arr => [...new Set(arr)];` |
| 83. Merge two objects, with the second object overwriting the first | `const mergeObjects = (obj1, obj2) => ({ ...obj1, ...obj2 });` |
| 84. Find the difference between two arrays | `const arrayDifference = (arr1, arr2) => arr1.filter(item => !arr2.includes(item));` |
| 85. Convert a string to an integer | `const toInteger = str => parseInt(str, 10);` |
| 86. Convert a string to a float | `const toFloat = str => parseFloat(str);` |
| 87. Remove a specific key from an object | `const removeKey = (obj, key) => { const { [key]: removed, ...rest } = obj; return rest; };` |
| 88. Count the number of occurrences of an element in an array | `const countOccurrences = (arr, value) => arr.filter(item => item === value).length;` |
| 89. Convert an array to a set | `const arrayToSet = arr => new Set(arr);` |
| 90. Create a function that delays execution by a given time | `const delay = (ms) => new Promise(resolve => setTimeout(resolve, ms));` |
| 91. Check if a value is a valid URL | `const isValidURL = url => /^(ftp|http|https):\/\/[^ "]+$/.test(url);` |
| 92. Check if a value is an array | `const isArray = value => Array.isArray(value);` |
| 93. Check if a value is a function | `const isFunction = value => typeof value === 'function';` |
| 94. Get the type of a value | `const getType = value => Object.prototype.toString.call(value).slice(8, -1);` |
| 95. Shuffle an array randomly | `const shuffleArray = arr => arr.sort(() => Math.random() - 0.5);` |
| 96. Generate a random number within a given range | `const getRandomInRange = (min, max) => Math.floor(Math.random() * (max - min + 1)) + min;` |
| 97. Calculate the factorial of a number | `const factorial = num => num <= 1 ? 1 : num * factorial(num - 1);` |
| 98. Check if a string contains a specific word | `const containsWord = (str, word) => str.includes(word);` |
| 99. Get the current date in a specific format | `const formatDate = (date, format) => { const options = { year: 'numeric', month: 'short', day: 'numeric' }; return new Date(date).toLocaleDateString(undefined, options); };` |
| 100. Remove leading and trailing spaces from a string | `const trimString = str => str.trim();` |
