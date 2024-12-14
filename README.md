# React Router Catch-all Route Issue

This repository demonstrates a common issue in React Router v6 where a catch-all route (`path="/*"`) unintentionally overrides other, more specific routes.  The problem arises when this catch-all route is placed after other routes, causing it to match all paths, even those already handled by other routes.

The issue is fixed by placing the catch-all route at the end of the routes definition.  This ensures that only paths not matched by more specific routes are caught by the catch-all route.
