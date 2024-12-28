# React Router v6 Catch-all Route Conflict

This repository demonstrates a common issue encountered when using catch-all routes ("/*") in React Router v6.  The problem arises when the catch-all route unintentionally captures paths intended for other routes, leading to unexpected behavior.

## Problem

The `App.js` file contains a simple React Router setup.  Notice that the catch-all route (`path="/*"`) interferes with other routes, and this should be avoided. This is commonly observed when the catch-all route is placed after more specific routes in the `Routes` component.  All requests should be handled by the specific routes first.