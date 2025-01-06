# React Native Unhandled JS Exception: Cannot read properties of undefined (reading 'name')

This repository demonstrates a common React Native bug and its solution.  The bug occurs when attempting to access a state variable or prop before it has been initialized, often during asynchronous operations like API calls.  This leads to an 'undefined' error when trying to access properties of the uninitialized variable.

The solution employs conditional rendering to check if the data has loaded before rendering components that depend on it.  Alternatively, the optional chaining operator (?.) can prevent errors if the data is undefined. 

## How to Reproduce

1. Clone this repository.
2. Run `npm install` or `yarn install`.
3. Run the app on your simulator or device.
4. Observe the error. 

## Solution

The solution is implemented in `bugSolution.js` and involves conditional rendering and/or optional chaining.