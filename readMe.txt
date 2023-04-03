1: What is the Event loop?

Ans: The event loop is what allows Node.js to perform non-blocking I/O operations — despite the fact that JavaScript is single-threaded — by offloading operations to the system kernel whenever possible.


2: Explain the 6 phases of the event loop

Ans

a. Timers: this phase executes callbacks scheduled by setTimeout() and setInterval().

b. Pending callbacks: executes input and output callbacks deferred to the next loop iteration.

c. Idle, prepare: only used internally.

d. Polling stage: retrieve new input and output events; execute input and output related callbacks (almost all with the exception of close callbacks, the ones scheduled by timers, and setImmediate()); node will block here when appropriate.

e. Check: setImmediate() callbacks are invoked here.

f. Close callbacks: Some close callbacks, e.g. socket.on('close', ...).

3: List some best practices in server-side code development

Ans

i. Focus on code quality
ii. Make the code more maintainable and more readable.
iii. Keep code small s that it can be scalable.
iv. Handle errors by writing and presenting relevant error messages to locate edge cases, improve application reliability, and debug.

4: What is NPM 

Ans:
npm stands for Node Package Manager. It’s a library and registry for JavaScript software packages

5: How do you initialize a package in npm: 

Ans:
A git package can be initialised by typing npm init on the terminal.

6: How do you run a script in the package.json?

Ans:
Once an npm script has been added to package.json, it can run it using the npm run command. e.g npm run <script-name>


7: Initialize a package if your choice, give it a name and install the following npm packages to it, express, mongoose, joi.