# Uncommon HTML Error: Incorrect DOM Manipulation
This repository demonstrates a common yet subtle error in HTML involving DOM manipulation.  The error arises from using incorrect methods or attempting to access elements that may not exist, leading to unexpected behavior in the rendered webpage.

## Bug Description
The `bug.html` file contains a simple HTML page with two paragraphs. A JavaScript snippet attempts to modify these paragraphs using `document.getElementByTagName()`.  However, `getElementByTagName` is misspelled as `getElementByTagName` causing the code to throw an error, preventing the intended styling changes from taking effect. 

## Solution
The `bugSolution.html` file provides the corrected code. It uses the correct method `document.getElementsByTagName()` and also applies error handling to gracefully handle cases where elements might not be found.

## How to Reproduce
1. Clone this repository.
2. Open `bug.html` in your web browser's developer console. Observe the error message.  The page won't display the styling changes correctly.
3. Open `bugSolution.html`. Observe the corrected output with the paragraphs successfully styled.