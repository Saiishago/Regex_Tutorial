# Matching an Alphanumeric Format

Welcome to a tutorial guide on Matching an Alphanumeric Format Resex (regular expression) in Computer Science using JavaScript. At the end of this tutorial, one will hopefully have a better understanding of Regex (Reqular Components) Components. Okay, now it is time to breakdown the components of a regex pattern made/designed to validate an alphanumeric format, explain how each part plays a role in ensuring an accurate/correct outcome.

## Summary

**_The Regex Discussed in this tutorial is Below:_**

```
(\W|^)po[#\-]{0,1}\s{0,1}\d{2}[\s-]{0,1}\d{4}(\W|$)
```

Components that will be discussed in this tutorial are; Anchors, Quantifiers, Grouping Constructs, Bracket Expressions, Character Classes, The OR Operator, Flags and Characte Escapes. For the purpose of this tutorial, the regex line above will be referenced to give a better understanding of regex, how it works and just so one has a better grasp of the material.

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

All Regular Expressions have two anchors; a beginning anchor and an ending anchor. 1. We use the caret [^] to indicate the beginning of a string. 2. We use the dollar sign [$] to indicate the ending points of a string. (\W|^)po[#\-]{0,1}\s{0,1}\d{2}[\s-]{0,1}\d{4}(\W|$) You can clearly see them in the regex that will be discussed in this tutorial. Think of it as ; Every sentence begins with a [C]apital letter and ends with a full stop [.].

### Quantifiers

Quantifiers allow you to specify how many of a character or character class should be matched. For example, you can use \* to match zero or more occurrences of the preceding character or character class, or + to match one or more occurrences of the preceding character or character class.

### Grouping Constructs

### Bracket Expressions

### Character Classes

Character classes allow you to define specific sets of characters that can be used in a search pattern. For example, you can use \d to match any digit (0-9), or \w to match any alphanumeric character (a-zA-Z0-9).

### The OR Operator

### Flags

Finally, regexes can also use flags to modify their behavior. These flags allow you to change how the regex behaves, such as making it case-insensitive or allowing it to match on multiple lines.

### Character Escapes

A character escape represents a character that may not be able to be conveniently represented in its literal form.

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)

\W matches any character that’s not a letter, digit, or underscore. It prevents the regex from matching characters before or after the number.
^ matches the start of a new line. Allows the regex to match the number if it appears at the beginning of a line, with no characters before it.
$ matches the end of a line. Allows the regex to match the number if it appears at the end of a line, with no characters after it.
[#\-] matches a pound sign or a hyphen after the letters po, and {0,1} indicates that one of those characters can occur zero or one times. The \- (which indicates a hyphen) must occur last in the list of characters within the square brackets.
\s matches a space, and {0,1} indicates that a space can occur zero or one times.
\d matches any digit from 0 to 9, and {2} indicates that exactly 2 digits must appear in this position in the number.
