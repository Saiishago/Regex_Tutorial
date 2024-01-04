# Matching an Alphanumeric Format

Welcome to a tutorial guide on Matching an Alphanumeric Format Regex (regular expression) in Computer Science using JavaScript. At the end of this tutorial, one will hopefully have a better understanding of Regex (Reqular Components) Components. Okay, now it is time to breakdown the components of a regex pattern made/designed to validate an alphanumeric format, explain how each part plays a role in ensuring an accurate/correct outcome.

## Summary

We use Regex to create complex patterns for matching and searching text. Below is one of those complex patterns that will
be used for the purpose of this tutorial.

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

(\W|^)po[#\-]{0,1}\s{0,1}\d{2}[\s-]{0,1}\d{4}(\W|$)

Regular Expressions are tools we use for matching a pattern in text, anchors are special characters in a regex (regular expression) and are used to define the position of a pattern inside an input string. Regex (regular expression) have two anchors; a beginning anchor and an ending anchor. It is important to make sure that the whole string matches the specific pattern instead of just one part of the pattern.

1. We use the caret [^] to indicate the beginning of a string.
2. We use the dollar sign [$] to indicate the ending points of a string.

You can clearly see them in the regex that will be discussed in this tutorial. Think of it as ; Every sentence begins with a [C]apital letter and ends with a full stop [.].

### Quantifiers

(\W|^)po[#\-]{0,1}\s{0,1}\d{2}[\s-]{0,1}\d{4}(\W|$)

Quantifiers allow you to specify how many of a character or character class should be matched.

- We can use an asterisk [*] to match zero or more occurrences of the previous character or character class.
- We use the plus sign [+] to match one or more occurrences of the previous character or character class.
- The question mark [?] is used to match zero or one occurrence of the previous character or character class.

### Grouping Constructs

(\W|^)po[#\-]{0,1}\s{0,1}\d{2}[\s-]{0,1}\d{4}(\W|$)

- We use parenthesis [()] to group expressions and [(?:)] groups experessions without capturing them. In this regex, we have [(\W|^)] and [(\W|$)].

### Bracket Expressions

(\W|^)po[#\-]{0,1}\s{0,1}\d{2}[\s-]{0,1}\d{4}(\W|$)

These are also called Character Classes, which is discussed below. Bracket Expressions play an important part a regex (regular expression), because they let/allow us to define characters that match a certain part of the string.

- The [\W] in the very beginning and also at the end of the regex (regular expression) shows to match all/any characters that is not a word.
- The [\s] is used to match charaters with whitespace.
- The [\d] will match any numder that is equal to [0-9], look how both [\d] are followed by a [{number}].

### Character Classes

(\W|^)po[#\-]{0,1}\s{0,1}\d{2}[\s-]{0,1}\d{4}(\W|$)

- We use square brackets ([]) to define a character class, in our regex example, you will find
  [#\-] and [\s-] inside square brackets.
- Character classes allow you to define specific sets of characters that can be used in a search pattern.
- You could use \d to match any digit (0-9), or \w to match any alphanumeric character (a-zA-Z0-9).

### The OR Operator

(\W|^)po[#\-]{0,1}\s{0,1}\d{2}[\s-]{0,1}\d{4}(\W|$)

We use it to match one of two options in a regex (regular expression) and we make use of the [|] symbol to separate both option, so as to not confuse the expression. In our expression we have the [(\W|^)] seen in the beginning of the expression and the [(\W|$)] at the end of the expression.

### Flags

(\W|^)po[#\-]{0,1}\s{0,1}\d{2}[\s-]{0,1}\d{4}(\W|$)

Flags are modifiers that are added to pattern in order to change how it matches, and are often put at the end of a regex (regular expression) and are displayed/come across as being loners because they are presented as single characters. Flags can be divided into smaller parts;

- Case-Insensitive = It matches both lowercase and Uppercase letters/characters.
- Global = It matches the whole pattern not just the one part.
- Ignore Whitespace = Pays no attention to the visible whitespace, makes it so it is easily readable.
- Sticky = It needs the pattern to match from the index shown/displayed by the regex (regular expression) object.
- Multiline = Lets the ^ and $ anchors we see at the start and at the end of the regex (regular expression) to match the beginning/end of a line.

### Character Escapes

(\W|^)po[#\-]{0,1}\s{0,1}\d{2}[\s-]{0,1}\d{4}(\W|$)

Character Escapes let you match certain characters prefixed by a backslash symbol[\], represents a character that cannot be conveniently represented in its actual form.

## Author

Salome Mphago is a Front-End Developer / Graphic Designer [SalomeM](https://github.com/)

[Matching an Alphanumeric Format](https://support.google.com/a/answer/1371417?hl=en#Match-an-Alphanumeric-Format) had this to say about Matching an Alphanumeric Format;

"\W matches any character that’s not a letter, digit, or underscore. It prevents the regex from matching characters before or after the number.
^ matches the start of a new line. Allows the regex to match the number if it appears at the beginning of a line, with no characters before it.
$ matches the end of a line. Allows the regex to match the number if it appears at the end of a line, with no characters after it.
[#\-] matches a pound sign or a hyphen after the letters po, and {0,1} indicates that one of those characters can occur zero or one times. The \- (which indicates a hyphen) must occur last in the list of characters within the square brackets.
\s matches a space, and {0,1} indicates that a space can occur zero or one times.
\d matches any digit from 0 to 9, and {2} indicates that exactly 2 digits must appear in this position in the number."
