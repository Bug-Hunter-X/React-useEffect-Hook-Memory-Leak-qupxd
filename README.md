# React useEffect Hook Memory Leak
This example demonstrates a common error in React's `useEffect` hook: missing a cleanup function in the return statement.  This can lead to memory leaks if not handled correctly.

The `bug.js` file contains the buggy code. The `bugSolution.js` file provides the corrected version.  The bug is that the `useEffect` hook doesn't return a cleanup function, which causes a potential memory leak if the component unmounts before the effect finishes.