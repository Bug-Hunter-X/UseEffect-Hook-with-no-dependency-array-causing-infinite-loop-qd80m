# React useEffect Hook Infinite Loop Bug

This repository demonstrates a common error in React applications involving the `useEffect` hook.  The example shows how omitting the dependency array in `useEffect` can lead to an infinite render loop.  The solution shows how to fix the problem by properly specifying the dependencies.

## Problem
The `useEffect` hook in the `bug.js` file is used to log the current value of the `count` state variable. However, because the dependency array is missing, the effect runs after every render, causing the component to re-render continuously and log 'Count:' repeatedly to the console. This creates an infinite loop and performance issues.