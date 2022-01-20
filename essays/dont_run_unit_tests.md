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

## Listen to annoying and unhelpful people

If you're repeatedly asking someone to do something and they keep neglecting to do it, what should you do?
One approach is to pursue various ways of making them do it; threats, cajoling, naming and shaming, punishment, reward.
Many people will recognize these patterns from their school - they might be one of the things schools instil in us most effectively.

A different way forward is to assume that the people who are refusing know what they are doing, and then re-examine our other assumptions.

Do engineers know whether or not the running of the tests they wrote, in different contexts such as on build machines or other people's dev boxes, is helping them find bugs and improve their code?
If it was successful, would they be expected to know?
