# Unnecessary Re-renders in useEffect Hook

This example demonstrates an issue where the `useEffect` hook in React causes unnecessary re-renders and console logs due to its execution after every render.  The solution shows how to optimize this to only run when the value of `count` changes.

## Problem

The provided `MyComponent` uses `useEffect` without dependencies. This means the effect runs after every render, even if the `count` hasn't changed, leading to performance overhead and excessive logging.