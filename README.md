# burger

This project contains a burger logger createed using MySQL, Node, Express, Handlebars and a proprietary ORM. 

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites
1. Node.js must be installed on local machine or host. See https://nodejs.org/en/download/ for instructions.
  
### Overview
1. The app folder structure is as shown below.

 ```
.
├── config
│   ├── connection.js
│   └── orm.js
│ 
├── controllers
│   └── burgers_controller.js
│
├── db
│   ├── schema.sql
│   └── seeds.sql
│
├── models
│   └── burger.js
│ 
├── node_modules
│ 
├── package.json
│
├── public
│   └── assets
│       ├── css
│       │   └── burger_style.css
│       └── img
│       │   └── burger.png
│       └── js   
│           └── burgers.js
│
├── server.js
│
└── views
    ├── index.handlebars
    └── layouts
        └── main.handlebars
```


1. The file `main.handlebars` is the main layout that is populated by `index.handlebars` and `burger-block.handlebars`.
2. The server is created by the script `server.js` and it is designated as the start script. It requires the npm package `express`.
3. This project uses the MVC design pattern where:
   * Model: `burger.js`
   * View:  `main.handlebars`, `index.handlebars`, `burger-block.handlebars`
   * Controller: `burgers_controller.js`
4. The proprietary secret sauce for our database mapping is in `orm.js`.


### Installing

1. To install source files use git to clone files from https://github.com/danhunlee/burger.
2. In a bash terminal or Visual Code terminal navigate to the directory that you downloaded the files from github.
3. Install the Node package (express) by entering the following in the terminal:   
    *npm install* 
4. (optional) If deploying to to a host such as Heroku perform the following:
   1. Navigate to the root project folder in a terminal.
   2. Enter the following command in the terminal:
   *git push heroku master*

### Operation
To view Burger page navigate to https://burgerhw1.herokuapp.com/.
The Burger app can be operated on the local host as instructed below.
1. Using a browser navigate to the main page:   
    *localhost:3000*  
2. In the left column *Burgers that I will devour!* Click the button *Devour it* next to a burger you wish to eat to move it to the *Burgers that I've devoured!* column.  
3. In the right column *Burgers that I've devour!* Click the button *Nah...* next to a burger you wish to put back to move it to the *Burgers that I will devour!* column. 
4. To add a new burger enter the name of the burger in the *Burger Name* text box and click the button *Add Burger*. Your new burger will be added to the *Burgers that I will devour!* column. 


## Running the tests

Validation of Burger app was perform using a chrome browser. Burger was run as directed in the previous section - **Operation**.  

### Break down into end to end tests

Source files have been extensively tested by displaying pages in Visual Code.

## Deployment

Navigate to https://github.com/danhunlee/burger to clone.

## Built With

* [Visual Studio Code](https://code.visualstudio.com/)

## In development
Implementing textual hints.

## Authors

* **Heon Lee**

## License

This project is not licensed.

