# Regex Introduction

Welcome to regex introduction. This will show you in a short few minutes, what my HRML tag regex is about.

## Summary

What is regex, this is regular expression also known as regex! In this example we will learn what regex is and how it can be used, for HTML tags.
Regex search a string of characters to make sure that it matches what your looking for.(ie. password, email, login). Which is looking for a certain pattern. You can also use regular expression to extract data.

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

The component uses regular expressions to search for the match and to render output.
The search pattern is a set of one or more regex that is applied to the specified input property to search for a match which takes two imputs.

### Anchors

The anchor is something about the string or the matching process, assert the current position in the string matches a determined location like the beginning or the end or middle.
`example: ( <\/_?(?![^>]_?\b(?:a|img)\b)[^>]\*?> ) which will look for all html tags other than 'a' tags and 'img' tags

### Quantifiers

A quantifier is a number of character or expression that matches.
` example: <div>; <section>;

### Grouping Constructs

This is by grouping content together with opening and closing tags
` example: <div>; <main> front end and backend of the tag

### Bracket Expressions

An expression is what is in brackets.
`For example: /<.+?>/
The < matches for a '<' character
The Dot '.' matches for a character except for line breaks
The '+' is a quntifier which match for 1 or more of the precding tokens
The '?' make quntifiers lazy, making it match the lease amount of characters as possible
and '>' matches the '>' character

### Flags

Flags (there are only 6 of them) are used to find certain strings in your code, most of these can only be used for javascript.
i - is a case-insensitive flag, it wont matter it you have a
B or b it will look for it.
g - this is looking for only the first match in your code and returns it.
m - this will look for match in many lines of code.
s - starts a dotall that will allow a dot . to match in newline characters
u- this is unicode flag
y- also known as the sticky flag it searches for the exact position in the code

### Character Escapes

this is for javascript content you can use
\r for a carriage return
\t - for a horizontal tab
\v for vertical tab
`\' for making single quotation marks this one could be used for html.

## Author

David Larsen: I like to code and learn everything about coding.
GitHub: https://github.com/Jaajarbinks
