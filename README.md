# JavaScript Loose and Strict Comparison with NaN and -0

This repository demonstrates the unexpected behavior of JavaScript's loose comparison (==) and strict comparison (===) operators when dealing with NaN (Not a Number) and -0 (negative zero).

## The Problem

JavaScript's loose comparison (==) does type coercion which leads to unexpected result, whereas the strict comparison (===) compares values and type, in which NaN is never equal to itself, even NaN, and -0 is equal to +0.

## The Solution

Always use strict equality (===) to avoid unexpected results caused by type coercion.  For NaN comparison, use Number.isNaN().

## Usage

Clone the repo and run `bug.js` to see the unexpected behavior. Then, examine `bugSolution.js` to see how to use Number.isNaN() for correct NaN comparison.