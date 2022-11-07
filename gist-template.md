# ZW-REGEX-TUTORIAL

This is a tutorial showing a regular expression (regex) for matching an e-mail value.

## Summary

This document will explain all of the components of the following regex for matching an e-mail value:

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

This regex was provided to us by our instructor material and we are to break down its components to explain what the regex means and how it was constructed.

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
There are two anchors in this regex for matching an email value: 

* `^` -matches the start of a string. This matches a position and not a character.
* `$` -matches the end of a string. This matches a position not a character.

For our regex, these two anchors start and end the matching email value.


### Quantifiers

* `+` -this quantifier matches one or more of the preceding tokens. For example: in `([a-z0-9_\.-]+)` the `+` indicates that the value should match and digit, letter, or `.` once or more

* `{2,6}`- this quantifier sets a minimum and maximum character value at a minimum or 2 characters and a maximum of 6 characters. For example: `([a-z\.]{2,6})` the quantifier is setting a minimum and maximum value for characters in this the set range provided.

### Grouping Constructs

This regex has multiple capture groups. Each capture group designated by `()` treats the context of the group as a single unit. Examples of these groups from our regex are below:

* `([a-z0-9_\.-]+)` 
* `([\da-z\.-]+)`
* `([a-z\.]{2,6})`

### Bracket Expressions

Bracket expressions represent the range of characters to be used in a value search. These ranges are stored in `[]` as the name suggests. Below are some examples from our regex:

* `[a-z0-9_\.-]` -this bracket expression searches for lower case letters a-z, number 0-9, and special characters like `_`, `.`, and `-`.
* `[\da-z\.-]` -this bracket expression searches for all digits, letters a-z, and special characters `.` and `-`.

### Character Classes

There are two character classes in this regex, one of which is touched on above:

* `[a-z0-9_\.-]` -this is a range, a group of values separated by a hyphen that show a range of searchable characters. For this example the range is lower case letters a-z and digits 0-9.  

* `\d` -this character class is shorthand for digits, or all digits.

### The OR Operator

The OR Operator in regex is written as `|` and describes logic outside of brackets. There are no OR operators in this regex.

### Flags

Some regex have flags at their end to define any additional functionality or at times limits for the regex. Our regex for matching an email does not include flags but here are examples of some below:

* `g` -retains the index of the last match, allowing subsequent searches to start from the end of the previous match.

* `m` -when the multiline flag is enabled, beginning and end anchors (^ and $) will match the start and end of a line, instead of the start and end of the whole string.

### Character Escapes

There is only one Character Escape in this regular expression: 

* `\.` -this component separates the `.` as a special character that is used in the search. For example in `[a-z0-9_\.-]` the `\.` is included in this bracket expression as a character that can be searched and matched.


## Author

* [Github](https://www.github.com/ZacharyWarnes)
* [email](mailto:zacharywarnes@gmail.com)
