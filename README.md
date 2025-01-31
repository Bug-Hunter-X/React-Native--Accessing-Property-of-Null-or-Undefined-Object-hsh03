# React Native: Accessing Property of Null or Undefined Object

This repository demonstrates a common error in React Native applications: attempting to access a property of a null or undefined object. This typically occurs when dealing with asynchronous operations, such as fetching data from an API, where the data might not be available immediately when the component renders.

The `bug.js` file shows the problematic code. The `bugSolution.js` file demonstrates how to effectively handle this situation using optional chaining and nullish coalescing operators.

## How to reproduce

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` to install dependencies.
4. Run `npx react-native run-android` or `npx react-native run-ios` to run the application.

You'll see the error in the console until the data is fetched and the app renders correctly.

## Solution

The solution involves using optional chaining (?.) and nullish coalescing (??) operators. Optional chaining allows you to safely access properties of an object without throwing an error if the object or any of its intermediate properties is null or undefined. Nullish coalescing provides a default value if the object is null or undefined.