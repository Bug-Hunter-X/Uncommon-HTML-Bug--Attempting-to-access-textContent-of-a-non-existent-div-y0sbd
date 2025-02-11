# Uncommon HTML Bug: Accessing textContent of Non-Existent Div

This repository demonstrates a subtle bug in HTML/JavaScript where attempting to access the `textContent` property of a non-existent div element results in a runtime error. The error's subtlety stems from the fact that the script continues to execute beyond the point of failure. This leads to only partial execution of the code.

## Bug Description

The `bug.html` file contains JavaScript code that attempts to access the `textContent` property of a div element with the ID `'nonExistentDiv'`, which does not exist in the HTML.  This will result in a runtime error.  Following this faulty line, another similar line tries to access a div that does exist, and this line does execute despite the first error.