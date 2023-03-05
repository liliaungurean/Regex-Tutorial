# Regex Tutorial on Matching an Email

Regular expressions can be used to find patterns of characters within a string. This also allows you to find and replace characters or sequence within a code. The regex I’ll be using describes matched character information for valid email addresses.


## Summary

This is the regex code that we will be anaylizing today is: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#Grouping-and-Capturing)
- [Bracket Expressions](#Bracket-Expressions)
- [Greedy and Lazy Match](#Greedy-and-Lazy-Match)

## Regex Components

### Anchors

The anchors are useed `^` to start of a string and `$` to end a string

### Quantifiers

This example uses `+` to communicate that there is another sequence to be matched as a greedy quantifier.  It also uses `{2,6}` as another greedy quantification to specify that the input must be a minimum of 2 characters and maximum of 6 characters. 


### Character Classes

This is a regular expression. JavaScript classifies the use of any digit from 0-9 when the character class `/d` is used.


### Grouping and Capturing

There are 3 groups being captured in this example. Group 1: Username of the Email account `[a-z0-9_\.-]`

Group 2: captures the domain name or email service being used; `[\da-z\.-]`

Group 3: captures the domain extension (ex. .com, .net, .edu); `[a-z\.]{2,6}`


### Bracket Expressions

There are 3 Bracket Expressions in the example. The information is opened and closed between brackets like this `[]`. This identifies which information is allowed to be matched.

Example 1: `[a-z0-9_\.-]` includes case sensitive characters from a-z, numbers 0-9, underscore, period and hyphens.

Example 2: `[\da-z\.-]` includes all digits, case sensitive characters a-z, period and hyphens

Example 3: `[a-z\.]` includes case sensitive characters a-z, and periods

### Greedy and Lazy Match

This example only used greedy quantifiers `+` and `{}`. That means that it allows the match to expand as long as it needs to. Lazy quantifications would appear as `+?` and `{}?` and this will direct the system to make the shortest matches.

## Author

My name is Lilia Ungurean. I love to Travel.

Github: [Lilia Ungurean](https://github.com/liliaungurean)
