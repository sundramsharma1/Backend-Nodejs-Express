<div align="center">
  
  ![GitHub repo size](https://img.shields.io/github/repo-size/sundramsharma1/Backend-Nodejs-Express)
  ![GitHub stars](https://img.shields.io/github/stars/sundramsharma1/Backend-Nodejs-Express?style=social)
  ![GitHub forks](https://img.shields.io/github/forks/sundramsharma1/Backend-Nodejs-Express?style=social)
  [![Twitter Follow](https://img.shields.io/twitter/follow/StarkSundram?style=social)](https://twitter.com/intent/follow?screen_name=StarkSundram)
  
  <br />
  <br />

  <h1 align="center">Backend (Node.js, Express.js)</h1> 
  <p>In this repo, we will learn about backend development using Node.js with Express.js in depth.</p>
</div>

<br />

## Prerequisites

Before you begin, ensure you have met the following requirements:
* [Node.js](https://nodejs.org/en) must be installed on your operating system.

### Run Locally

To run your program on your local machine, type this command in your command prompt and hit enter:

```bash
node <filename>.js
```
<h1 align="center"> Start </h1>
<br>

## Chapter_1(Basics)
* Process = Process command is use to get details about node which is install on your local machine
  
   ```bash
  node <-|
  process <-|
  ```
  * Process.argv = Process.argv is use to take command line argument to run our programm
  
  ```bash
  let n = process.argv;
  for(let i = 2; i < n.length; i++){
    console.log("Hiii", n[i]);
  };
  ```
* To run this program type this command on command prompt
   
  ```bash
  node <filename>.js <arguments>
  ```

   lets suppose i type this
  
    ```bash
    node process.js sundram mohit
    ```

   it will produce the output as
  
    ```bash
    Hii sundram
    Hii mohit
    ```

## Chapter_2 (Exporting File or Folder)
  * Require() = A built-in-function to include modules that exist in seperate files
  * Modules.export = A special object <br><br>
### Exporting a Single File =>
## Example => <br><br>
    
   File.js
    
   ```bash
   module.exports = 123;
   ```
   script.js
  
   ```bash
   const data = require('./File');
   console.log(data);
   ```
   O/P = 123

### Exporting a Entire Directories => 
##  Example => <br>
   * Folder Structure
     
     ```bash
            main/
           │
           ├── Fruits/
           │   ├── Apple.js
           │   ├── Banana.js
           │   ├── Orange.js
           │   └── index.js
           │
           └── script.js
     ```
   * Apple.js
     ```bash
     const apple = {
        name: 'Apple',
        color: 'Red',
        price: 90
     };

     module.exports = Apple;
     ```
     
  * Banana.js
    ```bash
    const Banana = {
        name: 'Banana',
        color: 'Yellow',
        price: 50
    };

    module.exports = Banana;
    ```
   * Orange.js
     ```bash
     const Orange = {
         name: 'Orange',
         color: 'Yellow',
         price: 60
     };

     module.exports = Orange;
     ```
  * index.js
    ```bash
    const apple = require('./Apple');
    const banana = require('./Banana');
    const orange = require('./Orange');

    module.exports = {apple, banana, orange};
    ```
   * Script.js
   ```bash
   const info = require('./Fruits');
   console.log(info);
   ```
   * O/P = <br>
    { <br>
    apple: { name: 'Apple', color: 'Red', price: 90 },<br>
    banana: { name: 'Banana', color: 'Yellow', price: 50 },<br>
    orange: { name: 'Orange', color: 'Yellow', price: 60 }<br>
    }
## Require() Vs Import
  ### Require() = 
  * We Can't Selectively load only the pices we need
  * It is a old method to load any file before (ES6)
  * It is used to load whole file at a time
  * module.exports = file_name;
  * In this method Loading is Synchronous Means line wise module loaded
  ### Import() = 
  *



































   
