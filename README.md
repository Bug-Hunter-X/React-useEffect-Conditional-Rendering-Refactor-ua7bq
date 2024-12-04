# Incorrect Conditional Rendering in useEffect Hook

This repository demonstrates a common bug in React applications involving incorrect conditional rendering logic within the `useEffect` hook. The bug causes the document title to not update properly when the count is 0.

## Bug Description

The `MyComponent` component uses the `useState` hook to manage a count.  The `useEffect` hook attempts to update the document title based on the `count` value. However, the conditional statement `if (count > 0)` prevents the title from updating when the count is 0, resulting in the title remaining unchanged from its initial state.

## Solution

The solution involves removing the conditional statement and updating the document title unconditionally within the `useEffect` hook. This ensures that the document title is always updated to reflect the current count value.