### Development Process

* #### Test Driven Development

![alt text](../img/dev-process.png)


### HOW IT WORKS!

1. `TEST FAILS` - Add a test, which will certainly FAIL

    - In TDD, every `functions`, `methods` and `components` in a software is first added in terms of test cases
    - Developers focus on the requirements before writing the code.
    - Run all the tests. See if any test fails

2. `TEST PASSES` - Write code 
    - add logical blocks to build the function

3. `REFACTOR` - Refactor the code
    - New code that might have been added for convenience to pass a test can be moved to its logical place in the code
    - Duplication must be eliminated
    - Object definitions and names must be set to represent their purpose and usage
    - As more features are added, functions become lengthy. It can prove beneficial to split and carefully named to improve readability and maintainability