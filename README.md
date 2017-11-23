[![](https://simondiep.github.io/img/node-multiplayer-snake.gif)](https://node-multiplayer-snake.herokuapp.com/)

A multiplayer snake game built on NodeJs, Express, socket.io, JavaScript ES6, and jspm using keyboard and gestures as controls.  No unnecessary libraries. 

Based on the project : https://github.com/simondiep/node-multiplayer-snake

Live demo [Here](https://node-multiplayer-snake.herokuapp.com/)

### Getting Started

Install the latest [Node.js](http://nodejs.org) 6 Stable

`git clone https://github.com/jgdrneto/snakeGame`

`cd snakeGame`

`npm install`

`npm run unbundle` This puts you into development mode, where hot deployments are possible.

`npm start`

Open your web browser to `localhost:3000`


### Game Features
 - Quick join and play (no sign-ups)
 - Player settings
   - Change colors
   - Change names
 - Admin controls
   - Change game speed
   - Add or remove bots
 - Different food types
 - Player statistics including kills/deaths/score
 - Steal player scores and length by killing them
 - Game notifications
 - Kill announcements
 - Randomized spawns
 - Spectate
 - Add and remove walls by clicking
 - Sound effects

### jspm notes
 - `npm run bundle` will bundle all of the js files together for a production environment
   - This updates `public/js/config.js` with an injected entry to load build.js
     - Don't check in the bundle changes to `public/js/config.js`
   - Any changes to javascript files after this will not be read, unless you bundle again or unbundle
 - Transpiling ES6 to ES5 is done on application load
 

### Technologies to look into
 - webpack vs jspm [Comparison](https://webpack.github.io/docs/comparison.html)
 - Replace console.log with logging framework
    - https://www.loggly.com/ultimate-guide/node-logging-basics/
    - https://strongloop.com/strongblog/compare-node-js-logging-winston-bunyan/
 - Unit test mocking frameworks for ES6 classes
 - Performance testing tools
 - Lightweight unit testing frameworks, such as [Tape](https://github.com/substack/tape)
 - ECMAScript 7
 