# Frontend Setup
For setting up the frontend for this project, we will be using [Neutrino](https://neutrino.js.org/), a tool that allows us to build web applications with minimal initial configuration. Neutrino is a wrapper around [Webpack](http://www.pro-react.com/materials/appendixA/), which is a tool that can analyze your project's structure, find JavaScript modules and other assets to bundle and pack them for the browser.

## Requirements
Before building a project with Neutrino, please make sure you have Node.js v6.9+ and npm installed.

## Getting Started
1. `cd` into the **senior-design** git repository on your local machine and run `git pull`. You will now have a file called **stockbox-frontend** in your project
2. Run `cd stockbox-frontend`
3. You can now execute the command `npm start` to build and run this project
4. You can now open **http://localhost:5000** in the browser to look at the application webpage

## Notes
I have configured Neutrino to use the test runner **Karma**. You can run `npm test` to execute tests for this project. 

## Additional Resources
* You can take a look at the [Neutrino docs] to learn more about how Neutrino works - although I do not expect that we will need to modify the setup much more than what I've alredy done.
* Do take a look at the documentaion on the [Project Layout](https://neutrino.js.org/project-layout.html) specified by Neutrino, as we will need to know that in order to modify the website.  
