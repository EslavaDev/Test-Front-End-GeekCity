# Test GeekCity Front
## Solving algorithm problems

### Example
array = [2,1,5,5,5,2]
The maximum height array are **5** units high. There are **3** of them, so return **3**.

### Function Description
arrayCalculate has the following parameter(s):
int arrays[n]: the array heights
### Returns
int: the number of array that are tallest
### Input Format
The first line contains a single integer, **n** , the size of array[].
The second line contains **n** space-separated integers, where each integer **i** describes the height of **array[i]**.

### Sample Input 0
> 4
> 3 2 1 3

### Sample Output 0

> 2

### Explanation 0

array heights are **[3,2,1,3]** . The tallest arrays are **3** units, and there are **2** of them.

```
'use strict';

const fs = require('fs');

process.stdin.resume();
process.stdin.setEncoding('utf-8');

let inputString = '';
let currentLine = 0;

process.stdin.on('data', function(inputStdin) {
    inputString += inputStdin;
});

process.stdin.on('end', function() {
    inputString = inputString.split('\n');

    main();
});

function readLine() {
    return inputString[currentLine++];
}

/*
 * Complete the 'arrayCalculate' function below.
 *
 * The function is expected to return an INTEGER.
 * The function accepts INTEGER_ARRAY candles as parameter.
 */

function arrayCalculate(array) {
    // Write your code here

}

function main() {
    const ws = fs.createWriteStream(process.env.OUTPUT_PATH);

    const arrayCount = parseInt(readLine().trim(), 10);

    const array = readLine().replace(/\s+$/g, '').split(' ').map(arrayTemp => parseInt(arrayTemp, 10));

    const result = arrayCalculate(array);

    ws.write(result + '\n');

    ws.end();
}

```

## Create React Web

### Description
you need a website where the user can start session and list the movies and know which are the user's favorite movies, the design is to your imagination, you need mobile first


### Requirements
- used Yarn
- used Creat React App
- used Typescript or JavaScript (but i prefer typescript)
- used React Hooks
- used Redux
- used firebase

### Will be qualified
- scalfollding
- design patterns
- store design
- coding optimization
- good practices
