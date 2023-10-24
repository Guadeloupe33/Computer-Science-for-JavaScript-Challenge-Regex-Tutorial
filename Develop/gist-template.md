# A Beginner's Guide to Regular Expressions (Regex)

## Introduction

Regular expressions, often abbreviated as "regex," are powerful tools for pattern matching and text manipulation in programming. They allow you to search for, match, and manipulate text based on specific patterns. In this tutorial, we'll explore the regex pattern for matching a URL and break down each component to understand how it works.

## Summary

In this tutorial, we will focus on the regex pattern for matching a URL: `^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$`. We will dissect this complex expression step by step, explaining the role of each part and how they come together to match URLs.

## Table of Contents

1. [Anchors](#anchors)
2. [Quantifiers](#quantifiers)
3. [OR Operator](#or-operator)
4. [Character Classes](#character-classes)
5. [Flags](#flags)
6. [Grouping and Capturing](#grouping-and-capturing)
7. [Bracket Expressions](#bracket-expressions)
8. [Greedy and Lazy Match](#greedy-and-lazy-match)
9. [Boundaries](#boundaries)
10. [Back-references](#back-references)
11. [Look-ahead and Look-behind](#look-ahead-and-look-behind)
12. [Author](#author)

## Regex Components

Now, let's explore the individual components of the regex pattern for matching a URL to understand what each part does.

### Anchors
Anchors in regex are used to specify the position of the pattern within the text. The `^` at the beginning and `$` at the end of our URL regex ensure that the pattern matches the entire string.

### Quantifiers
Quantifiers define how many times a character or group in the pattern should appear. In our URL regex, `*` and `?` are used to allow flexibility in the presence of certain parts, like the scheme and query parameters.

### OR Operator
The `|` symbol is used as an OR operator in regex. In our URL regex, it's used to separate two possible patterns for the scheme - with or without "https://" or "http://".

### Character Classes
Character classes represent a set of characters. In our regex, `[a-z]`, `[0-9]`, and `[.-]` are character classes. They match lowercase letters, digits, and period or hyphen characters, respectively.

### Flags
Flags like `i` can be added after the regex pattern to make it case-insensitive. In our example, we don't use any flags, but they are essential in other cases.

### Grouping and Capturing
Parentheses `()` are used to group and capture parts of the regex. In our URL regex, we use capturing groups to isolate the scheme, domain, and path.

### Bracket Expressions
Bracket expressions define a set of characters to match. They are used within character classes. In our regex, `[\/\w \.-]` is a bracket expression that matches a set of characters for the path.

### Greedy and Lazy Match
The `*` and `*?` quantifiers can be used to match text greedily or lazily. In our URL regex, `*` is used to match the path component greedily.

### Boundaries
Boundaries like `\b` can be used to specify the position at the beginning or end of a word. In our URL regex, we don't use boundaries, but they can be valuable in other cases.

### Back-references
Back-references allow you to match the same text that was previously captured in a capturing group. In our URL regex, we use capturing groups but not back-references.

### Look-ahead and Look-behind
Look-ahead and look-behind assertions allow you to match a pattern only if it is followed or preceded by another pattern. In our URL regex, we don't use look-ahead or look-behind.

## Author

This tutorial was created by Steven Francius. You can find more of my work and connect with me on GitHub.
(https://github.com/Guadeloupe33).
