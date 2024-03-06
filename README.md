# Regex Tutorial: Matching an Email

Welcome to my Regex Tuturial for Matching and Email. In this tutorial, we will explore the regular expression used to validate an email address. Email validation is a common task in web development and other applications where user input needs to be verified. Understanding how to use regular expressions (regex) for this purpose is essential.

## Summary

This tutorial will focus on the regex `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` for matching email addresses. We will break down each component of this regex and explain their purposes.

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

### Anchors

Anchors in regular expressions are used to specify the position of a match in the input string. The `^` anchor at the beginning of the regex ensures that the match starts at the beginning of the string. The `$` anchor at the end ensures that it ends at the end of the string.

### Quantifiers

Quantifiers specify the number of occurences of a character or a group in a pattern. In my regex, `+` is a quantifier that matches one or more occurences of the preceding character set.

### OR Operator

The OR operator in regular expressions is represented by the `|` symbol. It allows you to match either of two alternatives. But it is not explicitly used in this current example.

### Character Classes

Character classes allow you to match any one of a set of characters. In this example, `[a-z0-9_\.-]` matches any lowercase letter, digit, underscore, period, or hypen.

### Flags

Flags in regular expressions modify the behavior of the regex pattern. Common flags include `i` for case-insensitive matching, `g` for global matching, and `m` for multiline matching. However, in this example we are not using any flags.

### Grouping and Capturing

Grouping in regular expressions is done using parentheses `()`. Groups can capture parts of the match for later use. In my regex, there are three groups capturings the local part, domain, and top level domain of the email address.

### Bracket Expressions

Bracket expressions, or character classes, allow you to define the character sets for the local part and the domain part of the email address.

### Greedy and Lazy Match

In regular expressions, quantifiers are greedy by default, meaning they match as much as possible. To make them lazy, you can append `?` to the quantifier. However, in my example, I am not explicitly using lazy quantifiers.

### Boundaries

Boundaries in regular expressions allow you to specify where a match can occur in relation to word boundaries or other delimiters. Again, I am not explicitly using them in this expression.

### Back-references

Back-references allow you to reuse parts of a matched string within the regex pattern. They are represented by `\n`, where `n` is the index of the capturing group. My regex example does not include this.

### Look-ahead and Look-behind

Look-ahead and look-behind assertions allow you to assert that a pattern is or is not followed by another pattern without consuming the characters. My regex example does not include this.

## Author

This tutorial is authored by Kurstie DeHaven. You can find more projects and contributions on my Github Profile. @kurstiedehaven
