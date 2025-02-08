# React Router Dom: Unexpected Catch-All Route Matching

This repository demonstrates a common issue encountered when using React Router Dom's catch-all route (`/*`). The issue arises when the catch-all route unintentionally matches routes that should be handled by other, more specific routes.

## Problem

The problem is that the catch-all route (`/*`) will match any route not explicitly defined, even if a more specific route seems to be a better match.  This can lead to unexpected page renders and incorrect application behavior.  It often arises when route parameters or nested routes aren't properly considered.

## Solution

The solution involves careful ordering of routes and potentially using more specific route definitions to prevent the catch-all route from prematurely matching.

## How to reproduce

1. Clone this repository.
2. Run `npm install`
3. Run `npm start`
4. Observe that navigating to `/about` results in the expected About page.
5. The error is subtle; it's in the order and placement of the routes.