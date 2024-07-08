# Title (replace with your title)

In this gist, I will be going over regular expressions AKA regex. The point of this gist is to show off the different use-cases oof the many regex components and hopefully simplify it into a way that it can be easily understood.

## Summary

For example, when matching an Email the following regex code ( /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ ) will check the input string to make sure that:
1. Input characters are of acceptable aphanumeric value
2. There is an @ representing the origin of email
3. There is a . representing the type of site your email is originating from. (i.e: .gov, .com, .edu).
## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components
/^[a-z0-9_-]{3,16}$/
These are the general components of a regex. Most regex will contain at least one of these characters if not all.
### Anchors
^ - this anchor signifies a string that begins with the characters that come after it.
$ - this anchor signifies a string that ends with the characters that come before it.

### Quantifiers
*+?{}
These set limits on your stings. Limits such as maximum and minimum character requirements.
### OR Operator
(a|b|c)
This allows more flexibility with your string patterns, however the order of strings must stay the same.
### Character Classes
. - Matches any character in a line
 \d - Matches any Arabic numeral digit
 \w - Matches any Alphanumeric character including the underscore (_).
 \s - Matches a single whitespace character including tabs anf line breaks
### Flags
g i m
### Grouping and Capturing
(...)
### Bracket Expressions
[...]
### Greedy and Lazy Match
*? +? ?? {}?
### Boundaries
\b - word boundary
\y \Y - matches at any word boundary position
\M \m - matches at start of a word or end

### Back-references
\1
### Look-ahead and Look-behind
q(?!u) negative lookahead
q(?=u) positive lookahead
## Author

https://github.com/AkcCodes
AkcCodes is currently a student of the Full-Stack Web development course by way of the University of Minnesota.

