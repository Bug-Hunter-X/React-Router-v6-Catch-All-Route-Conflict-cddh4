# React Router v6 Catch-All Route Conflict

This repository demonstrates a common issue in React Router v6 where a catch-all route (`/*`) interferes with other defined routes. The catch-all route, intended to handle 404 errors, unexpectedly catches all routes, preventing other components from rendering.

## Problem

The provided `App.js` shows a basic React Router setup where a catch-all route (`/*`) is placed before other routes. This causes the catch-all route to always be matched, regardless of the URL, masking any other routes defined.

## Solution

The solution, provided in `AppSolution.js`, moves the catch-all route to the end of the `Routes` component. By doing so, it ensures that it will only match when no other route has matched, achieving the intended 404 handling behavior.
