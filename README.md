# PHP Infinite Recursion Bug

This repository demonstrates a common but subtle bug in PHP: infinite recursion. The `bug.php` file contains a function that processes data recursively. However, due to a lack of robust input validation and handling of edge cases, the function can enter an infinite loop if it receives unexpected input. This can lead to a stack overflow error, crashing the application.

The `bugSolution.php` file provides a corrected version of the function with improved input validation and error handling to prevent infinite recursion.

## How to reproduce the bug

1.  Run `bug.php`.
2.  Observe that if incorrect data is provided, the script may crash or run indefinitely.

## How to solve the bug

Review the code in `bugSolution.php` to see how input validation and handling of edge cases can prevent this type of infinite recursion.  Key improvements include better type checking, boundary checks, and base cases for recursion.