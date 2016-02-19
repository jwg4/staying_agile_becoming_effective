# The importance of TDD 

TDD is an important part of agile software development. Being agile usually means doing test-driven development in some form.
But it is also important because understanding the motivation for TDD helps us understand the motivation for other agile practices.
TDD is to 'writing code' as agile is to 'software development'.
This means that TDD can be a gateway drug for agile development in general.

## Why do TDD?
A lot of people have tried to answer this question. We hope that answering it will somewhat answer the question 'Why use agile practices?'
Inevitably a part of the answer is 'try it and you will be convinced'. 
We are very supportive of this approach, however we also sympathise with people who want the question answered *before* they try something new.
In this section we try to explain the theoretical answer.

TDD is a development method based on the principle that unit-tested code is easier to write than code without unit tests.
Before grokking TDD, developers can see the question of unit tests as a trade-off between code quality and speed of development.

In fact TDD represents a synthesis between the false dichotomy of 'getting the code out fast', and 'producing high quality code'.
The answer that TDD provides is not 'you should always produce high quality code', but 'tested and testable code is both 
quicker to develop and higher quality'.

The most important part of this is that adopting TDD does not mean 'writing the same code, but with tests'.
It means 'writing completely different code to solve the same problem': the reason that people insist that you try TDD
is that if you weren't writing tests first, it would be practically impossible to come up the the same code.
The unit tests are a by-product.
It should be obvious that this is the case - different development practices lead to different code.
The important thing we have to convince you of, is that the code you have written with TDD is *better* than the code you would have written without it.

## How TDD works.

Unlike the previous section, which explained the theory of how TDD is supposed to work, this one tries to show how it works in practice.
Here it is completely valid to suggest that you try doing TDD as well as reading about it, to understand exactly what doing TDD consists of.
There are lots of tutorials and suggested exercises for newbie TDD practictioners. 
One important part of this is that by trying TDD, you will get a sense of which problems TDD is simply great for,
and which problems is either doesn't help with as much, or simply is not valid for (yes there are some).
However, we respect your right to remain a TDD skeptic and not try it yourself until after you have read this section.

## But I already write code with a very low number of defects?

This question assumes that the purpose of TDD is to write code with fewer bugs.
Writing code with fewer bugs is a potential side-effect of TDD, not its purpose.
Some people already write code which is highly free of defects.
They do this either because they are very experienced at writing code, because they are very thoughtful about the code they write,
because they take the time needed to write high quality code, or some combination of these reasons. 
The purpose of TDD is
 - to make it easier and quicker to write this high quality code 
 - to make it easier and quicker to specify the behavior of the code
 - to make sure only the code that is needed is written
 - to make it easier and quicker to change this code in the future
 
 ## TDD is not making development quicker and easier!
 
 The obvious and extremely annoying answer to this is 'if it is not working for you, then you are doing it wrong'!
 This answer makes lots of sense to someone who is already a convinced TDD practioner, and no sense at all to someone who isn't yet.
 Instead it reinforces the idea that TDD, and by extension other agile practices, are some kind of brainwashing cult
 or pyramid scheme where everyone who is already a member promises to always pretend to outsiders that it is great.
 
 The real answer (which comes from a similar, but less irritating viewpoint) is that if TDD is not making development easier
 *you should stop doing it*. TDD is not like going on a diet, where you have to keep persisting with the pain until you
 start to see the gain. You should find writing code easier and be happier with the code you have written from the first 
 time you get a test to pass. If you don't, then the practices that you have adopted aren't working for you.
 Putting more and more effort into these failing practices will not make them start working.
 Instead you need to stop doing what you are doing, think again about how you do development,
 and then try and change your working methodology again in a different way.
 
