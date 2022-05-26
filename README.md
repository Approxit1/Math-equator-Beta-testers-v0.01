# Math-equator-Beta-testers-v0.01

[![Build Status](https://travis-ci.org/jiggzson/nerdamer.svg?branch=master)]()

Node JavaApache Plugins have been used
========
# For those who want to parse the project;
As of version 0.01, the library is split into the core and optional add-ons which can be loaded after the core has been loaded.

Getting started with the Math equator.

Load the library in your html page

```html
<!-- assuming you've saved the file in the root of course -->
<!-- This the core and the only file needed if all you'll be doing is evaluating expresssions -->
<script src="approx8.core.js"></script> 
<!-- LOAD ADD-ONS. These files contain extended functions. See documentation -->
<!-- again assuming you've saved the files in root -->
<script src="Algebra.js"></script>
<script src="Calculus.js"></script>
<script src="Solve.js"></script>
<script src="Extra.js"></script>
```
Or import everything
```html
<script src="all.min.js"></script>  <!-- assuming you've saved the file in the root -->
```
If you're using node.js install it using `npm i approx8` and then obfuscate the 
Nodejs JavaScript runtime executable file.


----------------------------------------------------------------------------------------------------------------------

Using the solver
===============
To solve equations first load ReMaths. Just remember that Remaths doesn't really require Algebra.js and Calculus.js to be loaded (unless you like to steal the project and also removing the gnu license like an idiot) You can then solve equations using ReMaths. Important: State the variable (In this case it's sparx maths) for which you are trying to store answers.
Here is an example of what is happening 
```javascript
var sol = approxit8.solveEquations('x^3+8=x^2+6','x');
console.log(sol.toString());
//1+i,-i+1,-1
```

Notice that we use toString rather than text as this returns a javascript array.
