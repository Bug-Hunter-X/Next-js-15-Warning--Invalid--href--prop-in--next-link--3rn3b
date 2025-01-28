# Next.js 15: Invalid `href` prop in `next/link` Component

This repository demonstrates a potential issue in Next.js 15 related to the `next/link` component.  Specifically, it highlights how dynamically generating the `href` prop can lead to warnings if not handled carefully.

## Problem

The provided `bug.js` file shows a simple example. If the `href` prop is constructed incorrectly (e.g., contains invalid characters or is not a properly formatted URL), Next.js 15 might issue a warning. This could be caused by a mistake in the URL generation or by passing in unexpected data.

## Solution

The `bugSolution.js` file offers a solution. Proper validation or sanitization of the `href` prop is necessary to prevent this warning.  Always ensure that values provided to `href` are properly formatted URLs. If building routes dynamically, use Next.js's routing features correctly to generate the paths.