# Jest-and-Testing-Library

# React Testing Library

Test the Software the way user actucally use it, not internal implementation but the working.
Find the elements by accessibility markers not by test IDs

# React Testing Library VS Jest

React Testing Library provides virtual DOM for tests( any time we are running the tests without browser, the test library provides a virtual DOM, so that we can test click elements and also whether the virtual DOM is behaving as what we want or not).
Jest on the other hand is the test runner that finds tests, run tests and determine whether test pass or fail.

# Assertions

These assertions are what determine whether the test passes or fails. So they are an essential part of the test function.

# Jest

React testing library, helps with rendering components into the virtual DOM using render method. It also helps with searching the virtual DOM, interacting with the virtual dorm, clicking on elements or entering text. However, it needs a test runner. It needs something that will find tests that will run them and will make assertions and that's where jest comes in. Jest as not the only test runner, there's Moka and then there's Jasmine, but jest as recommended by testing library, it also comes with Create React app and it is effective and easy to use. So when we ran NPM test in the terminal, we ran an NPM script that comes with Create React app and that script runs jest in watch mode.

# what is watch mode?

Watch mode is a way that you can run jest so that it will watch for any changes in files since the last commit and it will only run tests that are related to files that have changed since the last comment.

# How jest actually works, How does it know whethera test pastor failed?

There is a global test method that has two arguments, the first argument is a string description of the test and jest uses this argument and the second argument is a test function and jest runs that function to determine whether your test succeeds or fails.

# How does it do that?

Your test fails if any error is thrown while it's running that test function( The way assertions work is that they throw errors when your expectation fails). So if there's no error in the test function, then your test passes. So an empty test should pass.

#  types of tests.

The first type of tests are unit test, so this tests one unit of code, which is often a function or a react component in isolation. we don't want to test any interactions of this unit with any other units of code.

Integration tests, tests how multiple units work together, so that actually tests the interaction between units, so the interaction between components or the interaction between different micro services,

Functional tests are testing a particular function of the software. That function can mean a unit of your software that takes inputs

End to end tests, which we sometimes see written as E to E. These tests require an actual browser and they also require the server that your app is connected to. So these require a special tool, usually Cyprus or selenium.

