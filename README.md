# useRef Object Update Issue in React Native

This repository demonstrates a common, yet subtle, bug in React Native when using the `useRef` hook with an object as its initial value.  The object within `useRef` doesn't update correctly using the simple increment approach.

## Problem

The provided code snippet attempts to increment a counter within an object stored in a `useRef`.  However, it often does not update the displayed count correctly.

## Solution

The correct approach is to spread the current state and update it using the spread operator to create a new object, ensuring React re-renders properly. The solution file provides a corrected implementation.