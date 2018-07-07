## Node


### 1

1. Web workflow

    :question: The ___ is the physical hardware or software that takes requests from the ___ and gives something back or completes a process.
    * client, server
    * server, client
    * API, client
    * client, API

    <!-- answer 2 -->


### 2

1. More web workflow

    :question: Asking for something or some process to happen is called the ___ while what is returned as a result of it is called the ___.
    * request, response
    * AJAX, web page
    * response, request
    * request, API

    <!-- answer 1 -->


### 3

1. Server side development

    :question: ___ allows us to run JavaScript outside of the browser, and on the server instead.
    * HTTP
    * AJAX
    * Node
    * NPM

    <!-- answer 3 -->


### 4

1. Node server advantages

    :question: The advantage of using Node as a server is:
    * Easy extendability with plugins
    * Fast implementation with few lines of code
    * JavaScript use so frontend JavaScript devs can code backend too
    * all of the above

    <!-- answer 4 -->


### 5

1. Node server model

    :question: Node uses ___ threading which allows the server to handle all requests using a single thread through event-based callbacks.
    * perpendicular
    * synchronous
    * multi
    * asynchronous

    <!-- answer 4 -->


### 6

1. Executing JS files outside the browser

    :question: We can use Node to run a JavaScript file outside of the browser from bash/terminal with the command ___.
    * `node filename.js`
    * `run filename.js`
    * `filename.js execute`
    * You cannot - it must be run from the browser

    <!-- answer 1 -->


### 7

1. Console logging from Node

    :question: The file hello.js includes the code shown below. Where would the output be seen if hello.js was run using node from a bash/terminal window?
    ```JavaScript
    console.log('hello');
    ```
    * the browser window
    * the bash/terminal window
    * the browser's developer tools console
    * no output would be seen

    <!-- answer 2 -->


### 8

1. Purpose of process.argv

    :question: The process.argv property can be used to get all the ___.
    * files in the folder
    * active Node threads
    * command line arguments
    * bash/terminal process history

    <!-- answer 3 -->


### 9

1. Adding with process.argv

    :question: The file runMe.js contains the code shown below. What will be the output of executing the command `node runMe.js 5 5`?
    ```JavaScript
    console.log(process.argv[2] + process.argv[3]);
    ```
    * 5
    * 10
    * 23
    * 55

    <!-- answer 4 -->


### 10

1. parseFloat and parseInt

    :question: The parseFloat and parseInt JavaScript functions can be used to parse an argument into ___.
    * a number
    * a string
    * an array
    * a query

    <!-- answer 1 -->


### 11

1. Basics of modularization

    :question: When writing JavaScript files that use Node, we can bring in code exported from another file using the ___ keyword.
    * imports
    * module.imports
    * require
    * require.imports

    <!-- answer 3 -->


### 12

1. Modularization example

    :question: The file foods.js contains the code shown below. How would snickers be referenced in another file that had imported foods.js into the variable foods?
    ```JavaScript
    var yummies = {
        candy: "snickers",
        soda: "pepsi",
        chips: "lays"
    }

    module.exports = {
        yummies: yummies
    }
    ```
    * foods.yummies.candy
    * yummies.candy
    * foods.candy
    * foods.yummies

    <!-- answer 1 -->


### 13

1. Node FS package

    :question: The internal Node package ```fs``` is used for ___.
    * creating NPM packages
    * making AJAX requests
    * interacting with files
    * DOM updates

    <!-- answer 3 -->


### 14

1. Reading file data

    :question: The contents of the file data.txt are ```i,love,coding``` What will be the output of the code below?
    ```JavaScript
    var fs = require("fs");
    fs.readFile("data.txt", "utf8", function(err, data) {
        var output = data.split(",");
        console.log(output);
    });
    ```
    * ```i love coding```
    * ```i,love,coding```
    * ```['i', 'love', 'coding']```
    * ```{data: "i, love, coding"}```

    <!-- answer 3 -->


### 15

1. Adding to files

    :question: The ___ method of the Node ```fs``` package is used to add content to an existing file.
    * appendToFile
    * writeFile
    * continueFile
    * appendFile

    <!-- answer 4 -->
### 16

1. Adding pre-made code to Node apps

    :question: ___ allows us to quickly incorporate pre-made code snippets into Node applications.
    * The Node Package Manager
    * An API
    * GitHub
    * Web scraping

    <!-- answer 1 -->


### 17

1. Installing external packages

    :question: External packages needed by your Node app can be added with the command:
    * node install \<packagename\>
    * npm add \<packagename\>
    * node add \<packagename\>
    * npm install \<packagename\>

    <!-- answer 4 -->


### 18

1. Using the request NPM package

    :question: The code below shows an example of using the request NPM package to make a call to an API. Assume no API key is required. The useful data will be contained in the ___ variable as ___.
    ```JavaScript
    var request = require("request");
    request("http://www.omdbapi.com/?t=avatar", function(err, response, body) {
        // do something
    });
    ```
    * body, a JSON object
    * response, an array
    * err, an integer
    * body, string

    <!-- answer 1 -->


### 19

1. Purpose of JSON.parse

    :question: The JSON.parse() method parses a JSON ___, constructing the JavaScript object it describes.
    * object
    * array
    * string
    * module

    <!-- answer 3 -->


### 20

1. Package management

    :question: Any NPM packages that an application is dependent on should be listed in ___.
    * the package.json file
    * a readme file
    * the GitHub repository
    * a separate text file

    <!-- answer 1 -->


### 21

1. Adding dependencies

    :question: What command is used to create a package.json file?
    * npm add package.json
    * npm init
    * node package.json --save
    * node create --add --save

    <!-- answer 2 -->


### 22

1. Installing dependencies

    :question: When a Node application with correctly listed dependencies is shared, the subsequent developer can run the command ___ to re-download all the required NPM packages.
    * node install -all
    * npm add -all
    * npm install
    * node add dependencies

    <!-- answer 3 -->
