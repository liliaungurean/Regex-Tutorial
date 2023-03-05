# Regex Tutorial on Matching an Email
Introductory paragraph (replace this with your text)

## Summary

This is the regex code that we will be anaylizing today is: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#Grouping-and-Capturing)
- [Bracket Expressions](#Bracket-Expressions)
- [Bracket Expressions](#Bracket-Expressions)

## Regex Components

### Anchors

The anchors are useed `^` to start of a string and `$` to end a string

### Quantifiers

This example uses `+` to communicate that there is another sequence to be matched as a greedy quantifier.  It also uses `{2,6}` as another greedy quantification to specify that the input must be a minimum of 2 characters and maximum of 6 characters. 


### Character Classes

This is a regular expression. JavaScript classifies the use of any digit from 0-9 when the character class `/d` is uesed.

### Grouping and Capturing

There are 3 groups being captured in this example. Group 1: Username of the Email account `[a-z0-9_\.-]`

Group 2: captures the domain name or email service being used; `[\da-z\.-]`

Group 3: catures the domain extention (ex. .com, .net, .edu); `[a-z\.]{2,6}`

### Bracket Expressions

There are 3 Bracket Expressions in the example. The information if opened and closed betweent brackets like this `[]`. This identifies which information is allowed to be matched.

Example 1: `[a-z0-9_\.-]` includes case sensetive characters from a-z, numbers 0-9, underscore, period and hyphens. 

Example 2: `[\da-z\.-]` incudes all digits, case sensetive characters a-z, period and hyphens

Example 3: `[a-z\.]` incudes case sensetive characters a-z, and periods

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
