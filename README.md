# Regex Tutorial

In this tutorial, I will be explaining and demonstrating Regex (regular expressions) and how they work. We will break down each expression into manageable pieces that are easier to comprehend.

## Summary

In this tuotrial I will break down a regex for matching a email and explain what each pattern means.
The expression that will be used today is as followed: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

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
This expression is known as a literal so it will wrapped in / (foward-slash) characters.


### Anchors

Anchors, unlike literal characters and character classes, don't match any character. Anchors can be used to "anchor" the regex match to a certain position. 

Examples:

* `^` - matches any string that start with the preceding word
* `$` - matches a string that ends with preceeding word before the character
* Examples:
```
^Hello         - matches any string starting with "Hello"
World$         - matches any string ending with "World"
^Hello World$  - matches the exact "Hello World" string

### Quantifiers

Quantifiers specify the numbers of characters or expressions to match.

Examples:

x+ - matches the preceding item "x" 1 or more times. Equivalent to {1,}

### Grouping Constructs

Grouping combines a string to make the encased characters match in a unified block.

Examples:

- () - parentheses 
- (?:) - 


### Bracket Expressions

A bracket expression is a list of characters wrapped in the '[' and ']' brackets. The bracket expression matches any single character encased by the brackets. If the starting character is the caret '^', it matches any character NOT in encased by the brackets. 

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
OR Operators matches on of a selection of regular expressions: if you put the characters between any two characters in the expression, the output matches the combination of the strings that the two characters match.

Examples:

* `(|)` - matches a string that has any anterior characters followed by the characters on the left or right of the vertical bar
* `[]` - matches a string that has any anterior characters without any characters within the brackets

### Flags
Flags are specification that can be added on to an expression to make it differently discernable. Flags are placed at the end of a regex, after the second slash, and they define additional functionality for the regex. 

Examples:
'g' - global - searches for all instances
'm' -multi-line - combined with anchors, will only match the start and end of an expression

### Character Escapes
Any backslash (\) that is outside of a bracket [], escapes a character that if not would be transcribed literally.
In this expression the \. would show a example of this. 

## Author
Asha Sanford is a full stack web developer and animation gradute from Atlanta, GA. 
For more information or more repos, please visit my Github : https://github.com/ashasan1
