# Uncommon HTML Bug: Unexpected Number Assignment to innerHTML

This repository demonstrates a subtle bug in HTML related to the `innerHTML` property.  Attempting to directly assign a number to `innerHTML` results in unexpected behavior.  The solution shows the correct way to handle this.

## Bug Description
The code attempts to assign the number 123 to the `innerHTML` property of a div element. This results in the div becoming empty because `innerHTML` expects a string value, and the numeric value is treated differently. 

## Solution
The solution converts the number to a string using `String()` before assigning it to the `innerHTML` property. This ensures correct display of the numeric value.