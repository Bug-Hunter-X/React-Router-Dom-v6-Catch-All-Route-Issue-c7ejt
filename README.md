# React Router Dom v6 Catch-All Route Bug

This repository demonstrates a bug in React Router Dom v6 where the catch-all route (`/*`) overrides other routes, preventing them from rendering.  The issue occurs even when a more specific route should be matched first.  The solution demonstrates how to correctly implement a catch-all route.

## Bug

The `App.js` file contains the buggy code.  The catch-all route `/*` always triggers, even when `/` or `/about` should be matched.

## Solution

The `AppSolution.js` file contains the solution. The order of routes is crucial for correct functionality. More specific routes must appear before the catch-all route.