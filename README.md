# useEffect Hook Conditional Rendering Bug

This repository demonstrates a common bug related to conditional rendering within the `useEffect` hook in React. The bug arises from an incorrect condition causing unintended side effects or computations.

## Bug Description
The provided code uses a `useEffect` hook to log a message when the `count` state variable is greater than 0. However, the `useEffect` hook will always run due to the `count` being included in dependency array, and will unnecessarily log the message when count is 0.