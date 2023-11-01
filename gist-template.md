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

Quantifiers match instances of a character or group of characters.

```
*
```
The asterisk matches 0 or more instances of the preceding element.

```
+
```
The plus sign matches 1 or more instances of the preceding element. 

```
?
```
The question mark matches 0 or 1 instances of the preceding element. 

```
{2,6}
```
This quantifier specifies that the preceding pattern should be matched a minimum of 2 times and a maximum of 6 times

### Grouping Constructs

Grouping constructs are used to group characters together. They are grouped by using parentheses.

```
(https?:\/\/)?
```
This is an optional group matching the protocol of the url.

```
([\da-z\.-]+)
```
This group matches the URL subdomain and second-level domain.

```
([a-z\.]{2,6})
```
This group matches the top-level domain.

```
([\/\w \.-]*)*
```
this group matches any instances, if any, of a page path

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
