# React Native FlatList: Non-unique Keys Bug

This repository demonstrates a common bug in React Native's FlatList component: rendering issues caused by using non-unique keys.  The `FlatListBug.js` file shows the problematic code, while `FlatListBugSolution.js` provides the corrected version.

## Problem

When rendering a FlatList, each item *must* have a unique key. Using duplicate keys leads to unpredictable behavior, including incorrect item rendering, performance issues, and crashes. This is because React Native uses the keys to efficiently update the list.

## Solution

Ensure that each item in your FlatList data array has a unique key.  This usually involves using a unique identifier from your data source (e.g., an ID from your database).