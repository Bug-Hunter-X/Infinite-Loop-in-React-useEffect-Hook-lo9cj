# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications where an infinite loop occurs within the `useEffect` hook.

## Bug Description
The `MyComponent` component uses the `useEffect` hook to update the `count` state. However, the update occurs within the dependency array, leading to an infinite loop. 

## Solution
The solution involves correctly managing state updates within the `useEffect` hook, using the functional approach with a closure, or using a debounce function to avoid continuous updates. The corrected code demonstrates the functional approach to update the state with the previous state value.