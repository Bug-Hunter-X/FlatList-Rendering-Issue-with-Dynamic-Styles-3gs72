# React Native FlatList Dynamic Styling Bug

This repository demonstrates a common bug encountered when using FlatList in React Native with dynamic styles that depend on state updates. The bug manifests as incorrect styling or layout issues, particularly during scrolling or state changes. This README outlines the problem, its solution, and provides code examples to illustrate the issue and its resolution.

## Problem Description

When using FlatList to render items with styles derived from component state, inefficient updates can lead to rendering anomalies.  Changes in the component's state might not trigger the expected re-renders or cause inconsistencies in the displayed styles.

## Solution

The solution involves using `useMemo` and/or `React.memo` to optimize the rendering process and ensure that styles are calculated and updated efficiently, avoiding unnecessary re-renders and ensuring consistent styling.

## Code Examples

The `FlatListBug.js` file demonstrates the problematic code, and `FlatListBugSolution.js` offers the improved implementation.

## How to Run

1. Clone this repository.
2. Navigate to the project directory using your terminal.
3. Run `npm install` to install the project dependencies.
4. Run `npx react-native run-android` or `npx react-native run-ios` to start the app on your emulator or device. (Ensure you have React Native environment setup).

## Further Notes

This issue is a common pitfall when working with dynamic styles and state management in React Native. Understanding and applying efficient state management practices and memoization techniques is essential for building performant and reliable applications.