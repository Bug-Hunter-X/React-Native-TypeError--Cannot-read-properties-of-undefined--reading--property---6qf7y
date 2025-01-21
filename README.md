# React Native TypeError: Cannot read properties of undefined (reading 'property')

This repository demonstrates a common error in React Native: `TypeError: Cannot read properties of undefined (reading 'property')`.  The error arises when attempting to access a property of an object that is currently `undefined` or `null`. This often happens when dealing with asynchronous operations, where data might not be available immediately.

## Bug Reproduction

The `bug.js` file showcases the problematic code.  The app attempts to display the user's name from fetched data. If the fetch is still pending, accessing `user.name` will throw the error.

## Solution

The `bugSolution.js` demonstrates how to mitigate this error using optional chaining (`?.`) and nullish coalescing (`??`).  These features provide safe ways to access properties and handle potential null or undefined values.

## How to run

1. Clone the repository.
2. Navigate to the directory.
3. Run `npm install` to install the necessary dependencies.
4. Run `npx react-native run-android` or `npx react-native run-ios` to run the app on an emulator or device.

This example provides a practical understanding of the error and how to implement a robust solution in React Native.