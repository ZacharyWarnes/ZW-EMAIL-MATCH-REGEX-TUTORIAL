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

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
