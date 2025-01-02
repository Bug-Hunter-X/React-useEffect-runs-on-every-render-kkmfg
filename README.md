# React useEffect Runs on Every Render

This repository demonstrates a common issue in React applications where the `useEffect` hook runs on every render due to missing or incorrect dependency arrays.  This can lead to inefficient code and unexpected behavior.

## The Problem

The `useEffect` hook in the `bug.js` file lacks a proper dependency array.  Without it, the effect runs after every render, even if the state that the effect depends on hasn't changed. This can lead to unnecessary re-renders, increased load times, and unexpected side-effects.