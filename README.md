# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook and its dependency array. The bug causes an infinite loop, leading to performance issues and unexpected behavior.

## Bug Description

The `useEffect` hook is used to perform side effects, such as setting timers or fetching data.  The dependency array determines when the effect is triggered.  If the dependency array is incorrect or missing necessary dependencies, the effect may run repeatedly, creating an infinite loop.

## Bug Reproduction

The `bug.js` file contains the buggy code.  Observe the infinite loop when the component is rendered. This is due to the missing 'count' in the useEffect dependency array causing the effect to run on every render.