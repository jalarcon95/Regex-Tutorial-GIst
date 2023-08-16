# Regex Tutorial - Email Validation

This is a tutorial on how to use a Regular Expression (regex). They can be used to pull out information from a body of code. The Match Email regex can help with validating emails while using technologies such as Node. This tutorial will break down the components of the regex. Below, the table of contents can be used to quickly move to the topic the reader chooses.

## Summary

The following code snippet is used to match an email:

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

The above regex is a sequence of characters that define a search pattern. A regex can be used to validate input or find/replace characters within a string. This particular regex can be used to validate that emails are following the correct format.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors

Anchors can help mark the beginning and end of a regex. Instead of being used to match any characters, they are instead used to match a position before or after characters.

`^` - This anchor matches the beginning of a string or line

`$` - This anchor matches the end of a string or line 

### Quantifiers

Quantifiers match a number of instances of a character, group, or character class in a string. There are three quantifiers used in the match email regex. The quantifier matches the preceding token(character set).

`+` - This quantifier matches one or more times. Can be interpreted as {1, }. This quantifier appears twice in the example.

`{2,6}` - This quantifier matches specifically between 2 and 6 times. 

### Character Classes

A character class is used to match any symbol from a certain character set. Below, we will see what character classes are present in the example:

`\d` - Matches any single digit from 0-9. 

`a-z` - Matches any one lowercase letter from 'a' to 'z'.

### Grouping and Capturing

Grouping characters within (...) parantheses allows us to extract information for further processing or match text. Below, we see the captured groups from the exammple:

`([a-z0-9_\.-]+)` - Matches the email name. Anything the user puts before the '@'.

`([\da-z\.-]+)` - Matches the email domain. Examples include: gmail, yahoo, outlook, etc.

`([a-z\.]{2,6})` - Matches the top-level domain, which can have anywhere from 2-6 characters. Examples include: .com, .net, .us, etc.

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

John Alarcon Github: https://github.com/jalarcon95 Email: n/a

