# Incorrect Lifecycle Method for State Updates

This repository demonstrates a common error in React components where the wrong lifecycle method is used for updating the state after receiving new props.

## The Bug
The `BuggyComponent.js` file contains a React component that attempts to update its state using `componentDidMount`. This method only runs once when the component mounts and will not update the state when new props are received. 

## The Solution
The `FixedComponent.js` file corrects this issue by using the `componentDidUpdate` method to update the state only when the props have changed. This ensures the component's state correctly reflects the latest prop values.

## How to reproduce
1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Observe the unexpected behavior in the buggy component and then the correct behavior in the fixed component.