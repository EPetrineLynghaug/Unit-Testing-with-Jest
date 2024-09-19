# Lecture notes, Unit-Testing-with-Jest

## Description

This project demonstrates the principles and practices of Test-Driven Development (TDD). TDD is a software development approach where tests are written before the actual code. This method ensures that code functionality is verified at each step, making it easier to maintain, refactor, and debug as the project evolves.

In this project, we apply various testing types including Unit Testing, Integration Testing, End-to-End Testing, and others. The goal is to enhance the quality of code and reduce bugs by continuously verifying the code against pre-written tests.

## Key Features of TDD
<details>
  <summary><strong>Click to read more</strong></summary>

-  **Red-Green-Refactor Workflow:**  A core part of TDD, where a test is written first (Red), then the minimum code is written to pass the test (Green), and finally the code is improved or refactored (Refactor) without breaking the test.
- **Continuous Code Verification:** Tests are written before the code, ensuring that every functionality is verified immediately after implementation.
- **Incremental Development:** TDD encourages small, incremental steps in both test creation and implementation, promoting modularity and maintainability.
- **Error Detection:** TDD facilitates early detection of bugs and errors as tests highlight issues in real-time during development.
 </details>

## Advantages of Test-Driven Development
<details>
  <summary><strong>Click to read more</strong></summary>

1. **Improved Code Quality:**  Writing tests beforehand forces developers to think critically about the code’s functionality and edge cases, resulting in cleaner, well-structured code.
2.	**Reduced Bugs:**  By running tests continuously, TDD helps catch bugs early in the development cycle, making it easier to address issues before they escalate.
3. **Refactoring Confidence:** Developers can refactor their code with confidence, knowing that the tests will catch any unintended side effects of the changes.
4. **Better Code Design:** TDD naturally leads to better-designed code since it promotes small, testable, and decoupled modules.
5. **Documentation:** Well-written tests can serve as documentation for how the code is supposed to behave.

</details>

## Testing Types Used

<details>
  <summary><strong>Click to read more</strong></summary>

### 1. **Unit Testing**
- **Description**: Focuses on testing individual units of code, typically functions or methods, in isolation.
- **Libraries**: Jest, Mocha + Chai.
- **Example**: Testing a function that calculates a price or validates user input.

### 2. **Integration Testing**
- **Description**: Ensures that multiple components work together as expected. This could involve testing a DOM element or making an API call.
- **Libraries**: Jest + Testing Library, Cypress.
- **Example**: Testing if a form submission returns the expected result.

### 3. **End-to-End Testing (E2E)**
- **Description**: Simulates real-world user interactions with the application by automating browser tests.
- **Libraries**: Cypress, Puppeteer, Playwright.
- **Example**: Testing a full booking flow from user login to checkout.

### 4. **Component Testing**
- **Description**: Tests individual UI components in frameworks like React or Vue to ensure they work as expected.
- **Libraries**: Vue Test Utils, React Testing Library.
- **Example**: Testing a dropdown component to verify it behaves correctly.

### 5. **Snapshot Testing**
- **Description**: Ensures UI components do not change unexpectedly by capturing and comparing their rendered output to a stored snapshot.
- **Libraries**: Jest.
- **Example**: Verifying that a component’s style does not break after updates.

### 6. **Visual Regression Testing**
- **Description**: Detects visual bugs in the UI by comparing visual snapshots over time.
- **Libraries**: Chromatic, BackstopJS.
- **Example**: Ensuring that UI styles remain consistent after updates.

### 7. **Behavioral/Acceptance Testing (BDD)**
- **Description**: Simulates how end users interact with the system, often written in a more human-readable format.
- **Libraries**: CucumberJS.
- **Example**: Testing a user’s ability to log in, browse products, and add items to a shopping cart.

</details>

## Project Recommended Workflow

<details>
  <summary><strong>Click to read more</strong></summary>
   
The recommended workflow for frontend development in this project follows the TDD approach:

1. **Unit Testing**: First, we create unit tests to ensure that individual functions work as expected.
2. **Integration Testing**: We then ensure that different components work together correctly.
3. **End-to-End Testing**: Finally, E2E tests simulate a user interacting with the app to verify that the entire flow functions properly.
4. **Snapshot/Visual Regression Testing**: Lastly, visual tests are performed to ensure that UI components remain visually consistent over time.

</details>

## In This Project, We Aim To:
<details>
  <summary><strong>Click to read more</strong></summary>

- **Set up a basic TDD workflow**: Write tests before implementation and follow the Red-Green-Refactor cycle.
- **Implement multiple testing strategies**: Use unit, integration, and E2E testing.
- **Demonstrate common testing tools**: Showcase the usage of Jest, Mocha, Cypress, and other testing libraries.

</details>

## Tech Stack
<details>
  <summary><strong>Click to read more</strong></summary>

- **Node.js**: For running the testing environment.
- **Jest**: For unit and snapshot testing.
- **Cypress**: For integration and end-to-end testing.
- **React Testing Library/Vue Test Utils**: For component-level testing.
- **Babel**: For transpiling modern JavaScript.

</details>



## Example Tests
<details>
  <summary><strong>Click to read more</strong></summary>
   For demonstration purposes, we’ve created two simple test cases:

1.	**Addition Function:**  Tests both positive and negative number addition.
2.	**Subtraction Function:** Ensures that subtraction works correctly under various conditions.

</details>

## Setup Instructions
<details>
  <summary><strong>Click to read more</strong></summary>

1. **Install Node.js**: Ensure that you have Node.js installed. Run `npm init -y` to initialize the project.

2. **Install Dependencies**:
   ```bash
   npm install --save-dev jest babel-jest @babel/preset-env
   ```

3.	**Configure Babel:** Create a .babelrc file with the following:  
```json
 {
  "presets": ["@babel/preset-env"]
}
```


4.	**Run Tests:** Use the following command to run tests using Jest:
```bash
npm test
```
</details>


## Conclusion
<details>
  <summary><strong>Click to read more</strong></summary>
   Test-Driven Development (TDD) is a highly effective methodology that helps ensure code quality, reduce bugs, and promote modularity. By writing tests before implementation, developers are able to maintain a clear focus on the desired functionality and quickly detect issues as they arise. This project showcases several key types of testing—unit, integration, end-to-end, and more—providing a solid foundation for maintaining robust applications. The use of testing libraries such as Jest and Cypress, along with tools for visual regression and snapshot testing, enables continuous verification of both functionality and UI integrity. By following the TDD workflow, you can improve both the development process and the end product, ensuring a more reliable and maintainable codebase.

</details>