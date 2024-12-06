# React useEffect Infinite Loop Bug
This repository demonstrates a common bug in React applications involving the `useEffect` hook.  The bug stems from a missing dependency array, leading to an infinite re-rendering loop.

## The Problem
The `useEffect` hook in `bug.js` runs after every render because there is no dependency array.  This causes the `console.log` to continuously execute and the component to re-render endlessly, impacting performance significantly. 

## The Solution
The `bugSolution.js` file corrects this by adding the `count` variable to the dependency array. This ensures the effect only runs when the `count` value changes.

## How to reproduce
1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Observe the infinite logging in the console and potential browser freezing.

## How to solve
Examine the `bugSolution.js` for the corrected implementation.