# I automated something - and now it's a mess!

There is a whole set of theory about why code becomes, in a certain optimal limit, extremely similar in appearance to noise.
If we can predict the next character of a piece of text, then that character is redundant.
Most ways of writing computer code allow us to remove a lot of this redundancy using macros or definitions.
This process stops when either the language or the author enforce verbosity for the purpose of readability.
If neither do so, the code can become surprisingly close to noise while remaining meaningful (examples are often written in Perl or Q).

All this to say that it's somewhat natural for a list of instructions for carrying out a complex process to become extremely messy.
Imagine that you were given a set of instructions like this:

1. Open file A and replace yesterday's date with today's date. Copy the new total. Save the file.
2. Open file B and replace yesterday's date with today's date. Copy the new total. Save the file.
3. Open file C and replace yesterday's date with today's date. Copy the new total. Save the file.
4. Open file D and replace yesterday's date with today's date. Copy the new total. Save the file.

You would rightfully be annoyed and perhaps insulted. The author should have summarized the instructions, making them shorter, less redundant and less repetitive.

## Software is usually cleaner that this

## Interface design

Do-nothing scripts are a special case of upfront interface design: https://blog.danslimmon.com/2019/07/15/do-nothing-scripting-the-key-to-gradual-automation/

For some applications, arcane string commands are the correct interface.



## More automation doesn't make it less messy
