# Regex Tutorial

Regular expressions(regex) are a sequence of characters used to search for patterns in strings. This powerful tool can be used  for text processing, data validation, and searching for information in large data sets. In this guide, we'll take a closer look at the various components of regex and how they function.

## Summary
In this guide, we'll be discussing the following components of regular expressions:

- Anchors
- Quantifiers 
- OR Operator
- Character classes
- Flags
- Grouping and capturing
- Bracket expressions
- Greedy and lazy match
- Boundaries
- Back-references
- Look-ahead and look-behind

    Here is an example of a simple regex pattern that matches any alphanumeric string of length 7:
    ^[a-zA-Z0-9]{7}$


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors
- Anchors are characters that match specific positions in the input string. 
- There are two types of anchors in regex:`^` and `$`. 
- The `^` anchor matches the start of the line and the `$` anchor matches the end of the line.

### Quantifiers

- Quantifiers are characters that determine the number of times a character or group should be repeated in the input string.

#### The most commonly used quantifiers are:
 -  `*` (matches zero or more of the preceding character or group)
 -  `+` (matches one or more of the preceding character or group)
 -  `?` (matches zero or one of the preceding character or group)

### OR Operator

- The OR operator is represented by the pipe symbol `|` and is used to match either one expression or another. 
-   For example, the regex pattern `A|B` will match either an `A` or a `B` in the input string.

### Character Classes

- Character classes are defined using square brackets `[]` and match any single character that is contained within the brackets.
-  For example, the regex pattern `[abc]` will match either an `a`, `b`, or `c` in the input string.

### Flags

Flags are used to modify the behavior of the regex engine. 
#### The most commonly used flags are:
- `i` (case-insensitive)
- `m` (multi-line)
- `g` (global)

### Grouping and Capturing

- Grouping and capturing allow you to group multiple characters or patterns together and capture the matched text as a separate entity.
- Grouping is done using parentheses `()`
- Capturing is done by including the captured text in a separate group

### Bracket Expressions

- Bracket expressions are similar to character classes, but they allow you to specify a range of characters that should be matched.

### Greedy and Lazy Match
- Regex matching can be either greedy or lazy. A greedy match tries to match as much text as possible, while a lazy match matches as little text as possible. In other words, a greedy match tries to capture as much of the string as it can, while a lazy match tries to capture only what's necessary to satisfy the pattern.
- In regular expressions, a quantifier specifies how many times an element can be repeated. By default, quantifiers are greedy, meaning they will match as much text as possible. Lazy matching, on the other hand, matches as little text as possible.
- To make a quantifier lazy, you can add a `?` after it.
    - For example, the greedy quantifier `+` will match one or more occurrences of the preceding element, while `+?` will match one or more occurrences, but in a lazy manner.

### Boundaries

- Regex boundaries specify where a match can occur within a string
- For example, the `^` symbol matches the start of a line, while the `$` symbol matches the end of a line
    - These symbols help to ensure that a match only occurs where you expect it to.

    + Example:
        + ##### "Hello World" =~ /^Hello/ # matches "Hello" at the start of the string
            ##### "Hello World" =~ /World$/ # matches "World" at the end of the string
            ##### "Hello World" =~ /\bWorld\b/ # matches "World" as a complete word
### Back-references

- Back-references allow you to reuse a previously matched group within a regex. This can be useful for validating information, such as matching a password confirmation.

### Look-ahead and Look-behind
- Look-ahead and look-behind allow you to match a pattern only if it's preceded or followed by another pattern. For example, you might use a look-ahead to match a pattern only if it's followed by a specific word.

## Author
This tutorial was created by [Jay-MM](www.github/Jay-MM), a Junior Full Stack Developer.
