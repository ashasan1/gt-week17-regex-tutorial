# Title (replace with your title)

This tutorial will explain to users how regular expression, or regex, functions by breaking down each part of the expression and describing what it does.

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors

Anchors, unlike literal characters and character classes, and do not match any character at all. Anchors can be used to "anchor" the regex match to a certain position. 

Examples of Anchors are as follows:

* `^` - matches any string that start with the anterior word
* `$` - matches a string that end with preceeding word before the character
* Examples:
```
^Hello          matches any string starting with `Hello`
World$          matches any string ending with `World`
^Hello World$   matches exact string
goodbye         matches any string that has the exact text `goodbye` in it
```

### Quantifiers

Quantifiers indicate numbers of characters or expressions to match.

Examples:

x+ - matches the preceding item "x" 1 or more times. Equivalent to {1,}

### Grouping Constructs

Grouping combines a string to make it match in a unified block.


### Bracket Expressions

A bracket expression is a list of characters wrapped in the '[' and ']' brackets. The bracket expression matches any single character in that list. If the starting character is the caret '^', it matches any character NOT in that list. 

Examples:

- [0123456789] - matches any character between the brackets
- [^012345678] - matches any character NOT between the brackets

### Character Classes
Character classes are used to distinguish between the different types of characters, like distinguishing between letters and digits.

Examples: 

. - matches any character
\d - matches any numeral digit. Equal to 0-9
\w - matches any alphabetic or numeric character. Equal to A-Z, 0-9, and a-z
\S - matches a single charactr other than white space




### The OR Operator

### Flags
Flags are ______ that can be added on to an expression to make it search in a new way. 

### Character Escapes

## Author
Asha Sanford is a web developer and animation gradute from Atlanta, GA. 
For more information, please visit my Github : https://github.com/ashasan1
