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

Anchors do not match a character but match a position of a character. They are used to define where a match should occur and enforce location based constraints.

```
^
```
The caret matches the position before the first character in the string.

```
$
```
Similarly, the dollar sign matches the position after the last character in the string.

### Quantifiers

Quantifiers match instances of a character or group of characters. These specify how many times the preceding character or group of characters should occur. These can be combined with other regex elements to create complex expressions.

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

Grouping constructs are used to group characters together. They are grouped by using parentheses. Using grouping constructs allows the ability to treat one or more characters as a single unit.

```
(https?:\/\/)?
```
This is an optional group matching the protocol of the url. example: 'http://'

```
([\da-z\.-]+)
```
This group matches the URL subdomain and second-level domain.  example: 'post.techblog'

```
([a-z\.]{2,6})
```
This group matches the top-level domain. example: '.com'

```
([\/\w \.-]*)*
```
this group matches any instances, if any, of a page path. example: '/business'

### Bracket Expressions

Bracket expressions represent a range of character matches. These are represented with brackets.

```
[\da-z\.-]
```
This expression matches any digit (\d or [0-9]), any single character a-z (case sensitive), and any '.' or '-' characters.

```
[a-z\.]
```
This expression matches any single character a-z (case sensitive) and a '.' character.

```
[\/\w \.-]
```
This expression matches any word character (equivalent to [a-zA-Z0-9_])

### Character Classes

Character classes define a set of characters where any character in the set can validate a match.

```
\d
```
This class matches any numerical digit. Equivalent to [0-9].

```
\w
```
This class Matches any alphanumeric character from the basic Latin alphabet, including the underscore (_). Equivalent to [A-Za-z0-9_].

### The OR Operator

When matching for alternative patterns outside of a bracket expression the OR operator (|) is used. This is useful when looking for variations of a string or number. 

Examples:
* (yes|no) matches 'yes' or 'no' 
* (1|2|3) matches 1, 2, 3, and 321

### Flags

Flags are placed at the end of a regex and modify how the expression function.

```
g
```
Global search matching all occurances, not just one.

```
i
```
Enables case-insesitive matching.

```
m
```
Muli-line search.

### Character Escapes

Character escapes match literal characters and are represented with a foward slash.

```
\.
```
Matches a '.'

```
\/
```
Matches a '/'

## Author

This tutorial was created by Brian Pizzimenti, a passionate full-stack developer and enthusiast of all things related to technology and programming. Feel free to explore my GitHub profile for more useful resources, projects, and insights into the world of coding and software development. If you have any questions or feedback, don't hesitate to reach out to me on GitHub.
[GitHub](https://github.com/BrianPizz)  
