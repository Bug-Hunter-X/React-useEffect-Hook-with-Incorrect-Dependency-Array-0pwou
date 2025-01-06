# React useEffect Hook with Incorrect Dependency Array
This example demonstrates a common mistake when using the React `useEffect` hook. The effect is intended to log a message whenever the `count` state variable changes, however the dependency array is incorrectly set to `[]`. This results in the effect only running once upon initial component mount and not subsequently, even when the count changes.  The solution demonstrates the correct usage of the dependency array. 

## Bug
The bug is in the `MyComponent` function. The `useEffect` hook has an empty dependency array `[]`. This means that the effect will only run once, after the initial render.