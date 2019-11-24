global.browser = new BrowserHelpers()
* BrowserHelper class is a test tool for browsers that has several help methods as, clear cache, find buttons and titles, and also for debugging.

global.expect = chai.expect;
* Chai is an 'assertion library' for TDD compatible with node. Works with any js testing framework. I think that in that line we are telling the unit test that whenever we use 'assert', we use the one of Chai's.

 why we are placing "let fizzBuzz = new FizzBuzz" outside "it" block?
* fizzbuzz object can be used in all the tests inside the describe block.

difference between using === and == in JS?
* == compares 2 values, === compares values and datatypes

In  README  why we are moving (number % 5 === 0) to the top?
* Priority is for 5 if the number is both divisible by 5 or 3.

