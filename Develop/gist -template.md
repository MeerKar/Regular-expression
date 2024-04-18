# Regular Expression Sytanx(Regex)

A **regex**, which is short for **regular expression**, is a sequence of characters that defines a specific search pattern. When included in code or search algorithms, regular expressions can be used to find certain patterns of characters within a string, or to find and replace a character or sequence of characters within a string. They are also frequently used to validate input.

Regular expressions (regex) are powerful tool used in programming to search, match and maniplate text within patterns. They are used in various languages for validating, parsing and transforming text. Each component of a regex serves a specific purpose, enabling complex and flexible pattern matching.

## Summary

This is a walk through of fundamental components of regular expressions, often used for data validation, string manipulation, and complex text parsing. And will cover the syntax and function of anchors, quantifiers, grouping constructs, and more, with examples to demonstrate each concept.

Here is an example of a regex

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

Each component of this regex has a unique responsibility to make sure that a user enters an email address that begins with an unspecified number of characters preceding the `@` symbol, followed by a domain.

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

Anchors are used to match the position within the string.
The two anchors are `^` and `$`

. `^` represents the start of the string.
. `$` represents the end of the string.

### Quantifiers

Quantifiers specifies how many times a character, group or a character class must occur.

. `*`(0 or more)
. `+` (1 or more)
. `?` (0 or 1)
. `{n}`,`{n,}`,`{n,m}` (exactly n, at least n, between n and m)

### Grouping Constructs

Grouping Constructs are used to:

. Create subpatterns(`(abc)`)

. Apply quantifiers to parts of the pattern

. Create capture groups for extracting data from strings

### Bracket Expressions

Bracket expressions `[ ]` match any one character from a set of characters inside the brackets

.`[a-z]`matches any lowercase letter.
`[^a-z]` matches any character that is not a lowercase letter.

### Character Classes

Character classes provide a shortcut for common sets of characters

.`\d` matches any digit.

.`\w` matches any word of character
(alphanumeric and underscore).

.`\s`matches any white space character

### The OR Operator

The OR operator `|` allows for matching one of several subpatterns:

. `boy|girl` matches "boy" or "girl"

### Flags

Flags changes the behaviour of the regular expression

. `g` (global match)
. `i` (case insensentive)
. `m` (mutiline)

### Character Escapes

Character escapes allow you to match characters that are reserved as meta-characters in regex syntax:

. `\.` matches a literal dot.
. `\\` matches a literal backslash.

## Author

This guide is written by Meera Karnavar with the intention of helping developers and users to use regular expression in their projects
https://gist.github.com/MeerKar/90c5ff48e966b232a8196cf6b68ff3c5
