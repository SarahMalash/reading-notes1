# read 6:
## What Is Node.js?
JavaScript runtime built on Chrome’s V8 JavaScript engine.
*Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library*
## V8 engine:
 is the open-source JavaScript engine that runs in Google Chrome and other Chromium-based web browsers, including Brave, Opera, and Vivaldi.
 *compiling JavaScript directly to native machine code that your computer can execute.*
 *Node programs are executed in a browser*
 # creator of node:
  *(Ryan Dahl)* took the V8 engine and enhanced it with various features, such as a file system API, an HTTP library, and a number of operating system–related utility methods.
  
  Node comes bundled with a package manager called npm. To check which version you have installed on your system, type npm -v
  Installing a Package Globally and localy
  ## globaly:
  npm install -g jshint: This will install the jshint package globally on your system. We can use it to lint the index.js 
  ## localy: 
  npm init -y: This will create and auto-populate a package.json file in the same folder. 
  *Next*: use npm to install the lodash package and save it as a project dependency: npm install lodash --save
  Create a file named test.js and add the following:

const _ = require('lodash');

const arr = [0, 1, false, 2, '', 3];
console.log(_.compact(arr));
*Finally*: run the script using node test.js. You should see [ 1, 2, 3 ] output to the terminal.
#### What Is Node.js Used For?:
installing (via npm) and running (via Node) various build tools — designed to automate the process of developing a modern JavaScript application.
developing apps with any modern JavaScript framework
