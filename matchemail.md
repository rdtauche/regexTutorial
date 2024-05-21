# Regex Tutorial - Match Email

My assignment this week is to create a tutorial that explains how a specific regular expression, or regex, functions by breaking down each part of the expression and describing what it does. The bootcamp provided a template provided in the starter code to create my walkthrough.  I will be providing a tutorial on Matching an Email: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`


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
Anchors define specific positions in the string, such as the start or end.  In this example:  `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`, the ^ is the beginning anchor and $ is the end anchor.

### Quantifiers
Quantifiers specify how many times an element should be matched.  In this example, `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`, the: 
+ after [a-z0-9_\.-]: This quantifier specifies that the preceding character class must appear one or more times.
+ after [\da-z\.-]: This quantifier specifies that the preceding character class must appear one or more times.
{2,6} after [a-z\.]: This quantifier specifies that the preceding character class must appear between 2 and 6 times, inclusive.

### Grouping Constructs
Grouping constructs (i.e. parentheses) are used to create subpatterns and capture matches.  IN this example, `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`, the grouping constructs are the parentheses

### Bracket Expressions
Bracket expressions define a set of range of characters to match.  In this example, `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`, 
[a-z0-9_\.-]: This defines a character class that matches any lowercase letter, digit, underscore, period, or hyphen.
[\da-z\.-]: This defines a character class that matches any digit, lowercase letter, period, or hyphen.
[a-z\.]: This defines a character class that matches any lowercase letter or period.

### Character Classes
Character classes match any one character from a defined set

### The OR Operator
The OR Operator provies a choice between multiple patterns to match.  In the regex `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`, there is no OR operator (|). The OR operator is used to specify alternatives, such as in the pattern a|b, which matches either "a" or "b". This particular regex does not include such an alternation and focuses on matching the structure of an email address.

### Flags
Flags change the behavior of the regex, such as making it case-sensitive or enabling multi-line mode.  In the example `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` the regex pattern is enclosed in forward slashes (/) but does not include any flags after the closing slash.

### Character Escapes
Character escapes allow special characters to be treated as literals or match special character types.  In the regex `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`, there is one character escape:

\d: This escape sequence matches any digit (0-9).

## Author

Ross Tauchert has been in the banking industry for almost 20 years, working in the IT field for across foreign exchange, commodities and interest rates.  Ross is expanding his detailed knowledge of IT and working to become a full-stack developer.  Please find my github account here:  https://github.com/rdtauche

