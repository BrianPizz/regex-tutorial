# Regex Tutorial: Matching a URL

This tutorial will guide a user on how to use the following regular expression. 

## Summary

The regular expression, or regex, to match a URL is as follows:
```
/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/
```
This expressions checks to see if a string contains all the required characters of a valid URL. Each component will be broken down and explained.

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

Anchors do not match a character but match a position of a character. 

```
^
```
The caret matches the position before the first character in the string.

```
$
```
Similarly, the dollar sign matches the position after the last character in the string.

### Quantifiers

### Grouping Constructs

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
