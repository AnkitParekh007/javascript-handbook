# JavaScript Methods Reference

This project provides a comprehensive overview of commonly used JavaScript methods, grouped by their functionality, along with brief descriptions and usage examples.

## Document Object Model (DOM) Manipulation

| JavaScript Method          | Description                                           | Example                                                     |
|----------------------------|-------------------------------------------------------|-------------------------------------------------------------|
| `document.querySelector`   | Selects the first element that matches a CSS selector | `document.querySelector('.my-class')`                       |
| `document.querySelectorAll`| Selects all elements that match a CSS selector        | `document.querySelectorAll('.my-class')`                    |
| `getElementById`           | Selects an element by its ID                          | `document.getElementById('my-id')`                          |
| `getElementsByClassName`   | Selects all elements with a specified class name      | `document.getElementsByClassName('my-class')`               |
| `getElementsByTagName`     | Selects all elements with a specified tag name        | `document.getElementsByTagName('div')`                      |
| `createElement`            | Creates a new element                                 | `document.createElement('div')`                             |
| `appendChild`              | Adds a child element to a parent element              | `parentElement.appendChild(childElement)`                   |
| `removeChild`              | Removes a child element from a parent element         | `parentElement.removeChild(childElement)`                   |
| `replaceChild`             | Replaces an existing child element                    | `parentElement.replaceChild(newChild, oldChild)`            |
| `insertBefore`             | Inserts a new element before an existing element      | `parentElement.insertBefore(newElement, referenceElement)`  |
| `setAttribute`             | Sets an attribute on an element                       | `element.setAttribute('class', 'new-class')`                |
| `getAttribute`             | Gets the value of an attribute                        | `element.getAttribute('class')`                             |
| `removeAttribute`          | Removes an attribute from an element                  | `element.removeAttribute('class')`                          |
| `innerHTML`                | Gets or sets the HTML content of an element           | `element.innerHTML = '<p>New content</p>'`                  |
| `textContent`              | Gets or sets the text content of an element           | `element.textContent = 'New content'`                       |
| `style`                    | Gets or sets the inline style of an element           | `element.style.color = 'red'`                               |

## Event Handling

| JavaScript Method          | Description                                           | Example                                                     |
|----------------------------|-------------------------------------------------------|-------------------------------------------------------------|
| `addEventListener`         | Attaches an event handler to an element               | `element.addEventListener('click', function() { alert('Clicked!'); })` |
| `removeEventListener`      | Removes an event handler from an element              | `element.removeEventListener('click', functionName)`        |

## Class Manipulation

| JavaScript Method          | Description                                           | Example                                                     |
|----------------------------|-------------------------------------------------------|-------------------------------------------------------------|
| `classList.add`            | Adds a class to an element                            | `element.classList.add('new-class')`                        |
| `classList.remove`         | Removes a class from an element                       | `element.classList.remove('old-class')`                     |
| `classList.toggle`         | Toggles a class on an element                         | `element.classList.toggle('my-class')`                      |
| `classList.contains`       | Checks if an element contains a specified class       | `element.classList.contains('my-class')`                    |

## JSON Handling

| JavaScript Method          | Description                                           | Example                                                     |
|----------------------------|-------------------------------------------------------|-------------------------------------------------------------|
| `JSON.parse`               | Parses a JSON string into a JavaScript object         | `const obj = JSON.parse('{"name":"John"}')`                 |
| `JSON.stringify`           | Converts a JavaScript object to a JSON string         | `const jsonString = JSON.stringify({name: "John"})`         |

## Web Storage

| JavaScript Method          | Description                                           | Example                                                     |
|----------------------------|-------------------------------------------------------|-------------------------------------------------------------|
| `localStorage.setItem`     | Stores a key-value pair in local storage              | `localStorage.setItem('key', 'value')`                      |
| `localStorage.getItem`     | Retrieves a value by key from local storage           | `const value = localStorage.getItem('key')`                 |
| `localStorage.removeItem`  | Removes a key-value pair from local storage           | `localStorage.removeItem('key')`                            |
| `sessionStorage.setItem`   | Stores a key-value pair in session storage            | `sessionStorage.setItem('key', 'value')`                    |
| `sessionStorage.getItem`   | Retrieves a value by key from session storage         | `const value = sessionStorage.getItem('key')`               |
| `sessionStorage.removeItem`| Removes a key-value pair from session storage         | `sessionStorage.removeItem('key')`                          |

## Timing Functions

| JavaScript Method          | Description                                           | Example                                                     |
|----------------------------|-------------------------------------------------------|-------------------------------------------------------------|
| `setTimeout`               | Executes a function after a delay                     | `setTimeout(function() { alert('Hello'); }, 1000)`          |
| `setInterval`              | Repeatedly executes a function with a delay           | `setInterval(function() { alert('Hello'); }, 1000)`         |
| `clearTimeout`             | Clears a timer set with `setTimeout`                  | `clearTimeout(timeoutID)`                                   |
| `clearInterval`            | Clears a timer set with `setInterval`                 | `clearInterval(intervalID)`                                 |

## Fetch API

| JavaScript Method          | Description                                           | Example                                                     |
|----------------------------|-------------------------------------------------------|-------------------------------------------------------------|
| `fetch`                    | Makes a network request and returns a promise         | `fetch('https://api.example.com').then(response => response.json()).then(data => console.log(data))` |

## Promises

| JavaScript Method          | Description                                           | Example                                                     |
|----------------------------|-------------------------------------------------------|-------------------------------------------------------------|
| `Promise`                  | Creates a promise object                              | `new Promise((resolve, reject) => { if (condition) resolve('Success'); else reject('Failure'); })` |
| `then`                     | Adds fulfillment and rejection handlers to a promise  | `promise.then(value => console.log(value)).catch(error => console.error(error))` |
| `catch`                    | Adds a rejection handler to a promise                 | `promise.catch(error => console.error(error))`              |
| `finally`                  | Adds a handler to be called when the promise is settled | `promise.finally(() => console.log('Promise settled'))`     |

## Array Methods

| JavaScript Method          | Description                                           | Example                                                     |
|----------------------------|-------------------------------------------------------|-------------------------------------------------------------|
| `Array.from`               | Creates an array from an array-like or iterable object| `Array.from(document.querySelectorAll('div'))`              |
| `Array.isArray`            | Checks if a value is an array                         | `Array.isArray([1, 2, 3])`                                  |
| `Array.prototype.map`      | Creates a new array with the results of a function    | `array.map(x => x * 2)`                                     |
| `Array.prototype.filter`   | Creates a new array with all elements that pass a test| `array.filter(x => x > 10)`                                 |
| `Array.prototype.forEach`  | Executes a function once for each array element       | `array.forEach(x => console.log(x))`                        |
| `Array.prototype.reduce`   | Reduces array to a single value using a function      | `array.reduce((acc, cur) => acc + cur, 0)`                  |
| `Array.prototype.push`     | Adds elements to the end of an array                  | `array.push(4)`                                             |
| `Array.prototype.pop`      | Removes the last element from an array                | `array.pop()`                                               |
| `Array.prototype.shift`    | Removes the first element from an array               | `array.shift()`                                             |
| `Array.prototype.unshift`  | Adds elements to the beginning of an array            | `array.unshift(0)`                                          |
| `Array.prototype.slice`    | Returns a portion of an array as a new array          | `array.slice(1, 3)`                                         |
| `Array.prototype.splice`   | Changes array by removing/replacing elements          | `array.splice(1, 1, 'newElement')`                          |
| `Array.prototype.concat`   | Merges arrays                                         | `array1.concat(array2)`                                     |
| `Array.prototype.join`     | Joins array elements into a string                    | `array.join(', ')`                                          |
| `Array.prototype.indexOf`  | Finds the first index of a value                      | `array.indexOf('element')`                                  |
| `Array.prototype.find`     | Finds the first element that passes a test            | `array.find(el => el > 10)`                                 |
| `Array.prototype.findIndex`| Finds the index of the first element that passes a test | `array.findIndex(el => el > 10)`                           |

## String Methods

| JavaScript Method          | Description                                           | Example                                                     |
|----------------------------|-------------------------------------------------------|-------------------------------------------------------------|
| `String.prototype.charAt`  | Returns the character at a specified index            | `'string'.charAt(0)`                                        |
| `String.prototype.charCodeAt`| Returns the Unicode of the character at a specified index | `'string'.charCodeAt(0)`                                    |
| `String.prototype.concat`  | Joins two or more strings                             | `'Hello'.concat(' ', 'World')`                              |
| `String.prototype.includes`| Checks if a string contains another string            | `'Hello World'.includes('World')`                           |
| `String.prototype.indexOf` | Finds the first index of a value                      | `'Hello World'.indexOf('World')`                            |
| `String.prototype.lastIndexOf`| Finds the last index of a value                    | `'Hello World'.lastIndexOf('o')`                            |
| `String.prototype.match`   | Matches a string against a regex                      | `'Hello World'.match(/o/g)`                                 |
| `String.prototype.replace` | Replaces matches of a string with a new string        | `'Hello World'.replace('World', 'Everyone')`                |
| `String.prototype.search`  | Searches a string for a match                         | `'Hello World'.search('World')`                             |
| `String.prototype.slice`   | Extracts a part of a string                           | `'Hello World'.slice(0, 5)`                                 |
| `String.prototype.split`   | Splits a string into an array                         | `'Hello World'.split(' ')`                                  |
| `String.prototype.substring`| Extracts characters from a string                    | `'Hello World'.substring(0, 5)`                             |
| `String.prototype.toLowerCase`| Converts a string to lower case                    | `'Hello World'.toLowerCase()`                               |
| `String.prototype.toUpperCase`| Converts a string to upper case                    | `'Hello World'.toUpperCase()`                               |
| `String.prototype.trim`    | Trims whitespace from both ends of a string           | `' Hello World '.trim()`                                    |

This document provides a quick reference to commonly used JavaScript methods. For more detailed information, refer to the [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference).
