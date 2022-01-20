# I automated something - and now it's a mess!

There are lots of business processes which are carried out repetitively (once a day, every week, etc) and which involve some automation but also a considerable amount of human interaction.
In finance, think about reconciliations and regulatory submissions.
In engineering, think about releasing new versions.

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

When we automate, we often proceed bottom-up, starting from what needs to be done.

A common way of designing software is in the opposite direction, top-down.
This is a well-established methodology, which encourages us to write code that at initially looks like this:

```
def get_data():
    return None
    
def transform_data(d):
    return d
    
def write_data(d):
    pass
    
if __name__ == '__main__':
    d = get_data()
    t = transform_data(d)
    write_data(t)
```

Do-nothing scripts are a special case of upfront interface design: https://blog.danslimmon.com/2019/07/15/do-nothing-scripting-the-key-to-gradual-automation/
But lots of other interfaces are possible.
Suppose that a process has at least one step which requires manual/visual checking, correction or approval.
How can the interface be designed so that the person performing this manual step has as efficient and pleasant a workflow as possible?

For some applications, arcane string commands are the correct interface.

## More automation doesn't make it less messy

## Distinguishing removable complexity from intrinsic complexity

## Are long-term plans for reorganizing complex processes worthwhile?

Sometimes planning has a huge value, even though the plan is never carried out. At other times, it doesn't.

When we plan reorganizations, we go through the conceptual steps of understanding the whole process, and seeing it embedded in a process of change itself.
This usually means deciding which changes are possible within the constraints that the process must still be able to be run each day,
that data is preserved, that we can recover the process at the time to create old data, and so on.

As Doc admonishes Marty, we have to think four-dimensionally.

One difficulty, and in fact part of the reason that complex plans are needed, is that there is no infallible method for reshaping a hairy project into something that makes sense.
Plausible approaches include the following:
1. Making a single 'button push' which runs all of the process.
2. Building a dashboard or a task-and-issue queue so that someone carrying out the process only has to look in one place to know what to do next.
3. Merging different data models into a single schema or design.
4. Extracting and storing data from each part of the process.
5. Bringing disparate elements into one language, project or collection of code.
6. Making almost all elements subordinate to a single overarching one.
