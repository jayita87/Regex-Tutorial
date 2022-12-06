# Regex-Tutorial

A regular expression is a sequence of characters that specifies a search pattern in text. The patterns help you match, locate, and manage text.


## Summary

Emails are an ubiqutious form of communication amongst any platform. As an developer, it is important to verify that an user input is a valid email address
In this tutorial, we will be demonstrating regular expression for emails using: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/.


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)

## Regex Components

### Anchors
/`^`([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})`$`/
In regex, anchors are used to assert the current position in the string matches a well-determined location. In the regex code above, `^` anchor symbolizes the beginning of the text and `$` anchor symbolizes the end of the text.

### Quantifiers
/^([a-z0-9_\.-]+)@([\da-z\.-]`+`)\.([a-z\.]`{2,6}`)$/
In regex, quantifiers specify how many instances of a character, group, or character must be presented in the input for a match to be found. In the regex code above, `+` is a greedy quantifer that there is another sequence to be matched and `{2,6}` tells us that the input should be a minimum of 2 characters and a maximum of 6 characters.
### Grouping Constructs
The captures and groups include ([a-z0-9_\.-]+) to match the correct email name.
### Bracket Expressions
Bracket Expressions to validate an email address include [a-z0-9_\.-] to match letters, numbers, and characters within the brackets.
### Character Classes
A character class is  the set of characters that could occur in a string.  
The \d character class in the above code is looking for any digits, whereas a \D looks for non-digits, \s searches for space symbols, tab and newlines, \S looks for all but \s, \. any characters with the regex 's' flag, while the included \w character is looking for an alphanumeric character. 
### The OR Operator
The [] OR operator is used in this regex. For example, [a-z0-9_\.-] means any character a-z (case insensitive), any digit 0-9, _, ., or -. The \ is used to denote a literal . instead of the usual meaning of . which is "any character".
### Flags
The regex is enclosed by two / characters with no flags. Since multi-line is not enabled (by following the ending / with an m), the anchors match a string instead of the start and end of a line.
## Author
This tutorial was created by Jayita Chowdhury and you can find me <a href="https://github.com/jayita87">Github</a>