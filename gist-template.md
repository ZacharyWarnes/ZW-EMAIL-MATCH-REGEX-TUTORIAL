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


### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
