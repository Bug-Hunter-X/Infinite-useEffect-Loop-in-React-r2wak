# Infinite useEffect Loop in React

This repository demonstrates a common error in React applications: an infinite loop caused by an incorrectly implemented `useEffect` hook.

The `bug.js` file contains the erroneous code, while `bugSolution.js` provides the corrected version.

## Problem:
The `useEffect` hook in `bug.js` is missing a key dependency, causing it to re-run on every render and triggering an infinite render loop. 

## Solution:
The solution, in `bugSolution.js`, adds the `count` state variable to the `useEffect` dependency array. This ensures the effect only runs when the `count` variable changes.