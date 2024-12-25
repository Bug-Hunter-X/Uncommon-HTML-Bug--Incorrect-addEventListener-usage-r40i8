# Uncommon HTML Bug: Incorrect addEventListener Usage

This repository demonstrates a subtle bug in HTML related to the `addEventListener` method. The bug arises from incorrectly passing a string to `addEventListener` as the callback function instead of a function reference. This leads to unexpected behavior, where the event listener does not get properly attached.

## Bug Description

The bug lies in how the event listener is attached to the `div` element.  Instead of supplying a function reference, a string ("myFunction") is provided as the second argument to `addEventListener`. This is an incorrect usage, preventing the event from triggering the desired function.

## Bug Solution

The correct way to add an event listener is to provide the actual function reference as the second argument to `addEventListener`, not the function's name as a string.  The corrected solution below demonstrates the proper usage.