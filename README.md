# React Router Dom v6 Nested Routes Issue

This repository demonstrates a bug in React Router Dom v6 where nested routes fail to render correctly when their parent route is a wildcard route ("*...").

## Problem

When the parent route is a wildcard route, navigating directly to child routes using their respective paths does not render the child components.  The child routes only render if navigated to from the parent route.

## Solution

The solution involves using a different approach to handle nested routes, avoiding direct nesting under the wildcard parent route. The example provided in this repository showcases a working solution that uses a separate route for the fallback page (404).