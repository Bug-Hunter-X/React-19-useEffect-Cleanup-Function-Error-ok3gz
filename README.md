# React 19 useEffect Cleanup Function Error

This repository demonstrates a common error in React 19's `useEffect` hook where the return statement is missing a cleanup function in an effect that should only run once during mount.  This can lead to memory leaks and unexpected behavior.

## Problem
The `useEffect` hook in `bug.js` is designed to run only once on mount. However, the return statement is missing or incorrectly implemented, causing potential issues.

## Solution
The corrected version in `bugSolution.js` demonstrates the proper way to use a cleanup function within the return statement. This ensures that any side effects created by the effect are cleaned up properly when the component unmounts or when the effect is replaced by another.

This is crucial for performance and preventing unintended consequences, especially in complex React applications.