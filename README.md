# example-learn-js-app1
Example of web application using Node.js, express and MongoDB from Udemy's "Learn JavaScript: Full-stack from scratch" course.

This is a "To-do list" app.

It uses Node.js and express to set up a server that sends a HTML code to build a webpage with a form to input data that is displayed as a To-do list, loads and displays items stored in a database.
It has an edit and a delete feature for each of the list's items. The string data of each item of the list is stored in a MongoDB database with a simple free account.

The application can be run locally or hosted at Heroku, thus making it acessable on the internet via a specific http address.

This code has two main files: 'server.js' and 'browser.js'

server.js uses the express module and Node.js to initiate the server. It also contains the main html code embeded (this was done for example purposes only and it is understood that this is not clean code or a good coding practice). Moreover, the file connects to the MongoDB database, sets a password protected authorization layer and defines the 'create-item' POST method, the 'update-item' POST method and the 'remove-item' POST method.

browser.js (inside the 'public' folder) basically is responsible for the webpage rendering. It loads the HTML code of the page according to the information stored in the data base.

The application uses nodemon to automatically refresh the server as soon as any changes are made to the sourcecode files.
