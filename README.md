  <div align="center">
  
  ![GitHub repo size](https://img.shields.io/github/repo-size/sundramsharma1/Backend-Nodejs-Express)
  ![GitHub stars](https://img.shields.io/github/stars/sundramsharma1/Backend-Nodejs-Express?style=social)
  ![GitHub forks](https://img.shields.io/github/forks/sundramsharma1/Backend-Nodejs-Express?style=social)
[![Twitter Follow](https://img.shields.io/twitter/follow/StarkSundram?style=social)](https://twitter.com/intent/follow?screen_name=StarkSundram)
<br />
<br />

<h2 align="center"> Backend (Node.js, Express.js) </h2> 
In this repo we will learn about backend in node.js with express.js  in depth
</div>
<br />

### Prerequisites
Before you begin, ensure you have met the following requirements:
* [Node.js](https://nodejs.org/en) must be installed on your operating system.
  
### Run Locally
To run your Program on your local machine type this command on your command prompt and hit enter <br>

```bash
node <filename>.js
```
<h1 align="center"> Start </h1>
<br>

### Chapter_1
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
  To run this program type this command on command prompt
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
   
