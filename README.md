# React useEffect Infinite Loop

This repository demonstrates a common error in React's `useEffect` hook: an infinite loop caused by a missing dependency.  The `useEffect` hook runs after every render. If a value used inside the `useEffect` isn't included in the dependency array, React will re-run the effect every single time, potentially creating an infinite loop and crashing your app.