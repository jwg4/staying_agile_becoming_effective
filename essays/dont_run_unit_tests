# Stop running all your unit tests before deploying

TDD requires that, every time we write a line of code, we gather our thoughts and prepare to evaluate what we are about to write,
by first adding a test which will validate our implementation, based on an example of desired behavior. Several years later, when
we want to deploy to production some change to any piece of code in the same codebase (or even a non-code, non-unit-tested change
such as config), we run that same unit test we used to direct our thinking on that day, and only go ahead with deployment if it 
passes. Why?

## Analysis of TDD

This is not an anti-TDD essay. Firstly I love TDD, and secondly there are lots of good anti essays out there.
TDD means that your unit tests should be run, by the developer, at the time of writing the code, and each time that she modifies it
subsequently. Taking those unit tests and running them at some other time is neither required nor recommended by TDD.

TDD makes subordinate to the task of writing correct code which does what was intended by the developer, the task of writing decent
future-proof and maintainable tests which will allow you to validate your software's behavior. This is clear from how TDD works. 
