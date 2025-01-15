# Tcl List Index Out of Bounds Error

This repository demonstrates a common error in Tcl when working with lists: accessing elements outside the valid index range.  The `get_element` procedure attempts to access a list element using an index.  If the index is out of bounds, it should return an error code (-1 in this example). However, this implementation lacks robust error handling.

## Bug

The `bug.tcl` file contains the faulty `get_element` procedure that lacks complete error handling.  When an invalid index is passed, it doesn't handle it gracefully.  This can lead to unexpected results or crashes.

## Solution

The `bugSolution.tcl` file provides a corrected `get_element` procedure.  This version includes comprehensive error handling and returns an appropriate error code when an invalid index is used.
