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

Difference between feature and unit test.



Explaination for-
describe('User can input a value and get FizzBuzz results', () => {
    before(async () => {
        await  browser.init()
        await  browser.visitPage('http://localhost:8080/')
    });

    beforeEach(async () => {
        await  browser.page.reload();
    })

    after(async ()=> {
        await  browser.close();
    })
})
* when we try to run a feature test case , it does follwing functions.
@ Before running test it initialise and loads the browser.
@ Before running each test cases the browser is reloaded.
@After running test cases the browser is expected to close.

Explain the following-
it('clicking on the "Check" button', async () => {
    await browser.fillIn("input[id='value']", { with:  "3" })
    await browser.clickOnButton("input[value='Check']")
    let content = await browser.getContent("[id='display_answer']")
    expect(content).to.eql('Fizz');
})
* It is a test case to varify 'Fizz' is displayed if '3' is entered.In the test case ,fill the value with the '3'  and the check  button is cicked . The browser gets the value  displayed and compare it with 'Fizz'.



