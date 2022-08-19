# Regex Introduction

Welcome to regex introduction. This will show you in a short few line introduction to what regex is and how to use it.

## Summary

What is regex, this is regular expression also known as regex! In this example we will learn what regex is and how it can be used.
Regex helps to search for a string of characters to make sure that it matches.(ie. password, email, login). This is looking for a certain pattern.

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

This is the element that will be used to search for a string of characters to make sure that it matches.
example: [], ^, $, |, ()

### Anchors

string anchor () matches at the start of the string pattern
line anchor () matches after each line break with the start of a string pattern, also for the syntax weather it starts at the start or the end of the string
attempt anchor \`starts athe the start of the match attempt.

### Quantifiers

This specify how many instances of a character, group, or character class must be present in the input for a match to be found.

- \*? Matches zero or more times.

* +? Matches one or more times.
  ? ?? Matches zero or one time.
  { n } { n }? Matches exactly n times.
  { n ,} { n ,}? Matches at least n times.
  { n , m } { n , m }? Matches from n to m times.

### Grouping Constructs

This is delineate the subexpressions of a regular expression and capture the substrings of an input string.
They have capturing and noncapturing

Capturing- use parentheses are numbered automatically from left to right based on the order of the opening parentheses in the regular expression, starting from one. The capture that is numbered zero is the text matched by the entire regular expression pattern.

Noncapturing- is typically used when a quantifier is applied to a group, but the substrings captured by the group are of no interest.

### Bracket Expressions

This is either a matching list expression or a non-matching list expression.
It consists of one or more expressions: ordinary characters, collating elements, collating symbols, equivalence classes, character classes, or range expressions. The <right-square-bracket> ( ']' ) shall lose its special meaning and represent itself in a bracket expression if it occurs first in the list (after an initial <circumflex> ( '^' ), if any). Otherwise, it shall terminate the bracket expression, unless it appears in a collating symbol (such as "[.].]" ) or is the ending <right-square-bracket> for a collating symbol, equivalence class, or character class. The special characters '.', '\*', '[', and '\\' ( <period>, <asterisk>, <left-square-bracket>, and <backslash>, respectively) shall lose their special meaning within a bracket expression.

### Character Classes

This is any letter that is set inside of a bracket ([]),
example: [abcdefg....]

### The OR Operator

You can use an or operator to match characters or expression of either the left or right of the | operator. For example the (t|T) will match either t or T from the input string.
[j|J] will match j, J and |. You should either use (j|J), or [jJ].

### Flags

Regex has flags that affect the search.
there are 6 of them.

i
With this flag the search is case-insensitive: no difference between A and a (see the example below).
g
With this flag the search looks for all matches, without it – only the first match is returned.
m
Multiline mode (covered in the chapter Multiline mode of anchors ^ $, flag "m").
s
Enables “dotall” mode, that allows a dot . to match newline character \n (covered in the chapter Character classes).
u
Enables full Unicode support. The flag enables correct processing of surrogate pairs. More about that in the chapter Unicode: flag "u" and class \p{...}.
y
“Sticky” mode: searching at the exact position in the text (covered in the chapter Sticky flag "y", searching at position)

### Character Escapes

The \ is known as the escape code, which restore the original literal meaning of the following character.
The characters listed above have special meanings in regex. To match these characters, we need to prepend it with a backslash (\), known as escape sequence. For examples, \+ matches "+"; \[ matches "["; and \. matches ".".

Regex also recognizes common escape sequences such as \n for newline, \t for tab, \r for carriage-return, \nnn for a up to 3-digit octal number, \xhh for a two-digit hex code, \uhhhh for a 4-digit Unicode, \uhhhhhhhh for a 8-digit Unicode.

## Author

David Larsen: I like to code and learn everything about coding.
GitHub: https://github.com/Jaajarbinks
