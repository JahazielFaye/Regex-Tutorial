# Regex Tutorial: Matching Phone Numbers

## Introduction

Regular expressions (regex or regexp) are a powerful tool for pattern matching. They are a sequence of characters that define a search pattern. In this tutorial, we will be exploring how to match phone numbers using regex.


## Summary
This regex is used to match phone numbers in various formats including with or without country code, with or without spaces, dots or dashes. Let's break it down into its components and explain what each component does.

/^+?(\d{1,3})?[-. ]?\d3?\d3?[-. ]?\d{3}[-. ]?\d{4}$/

This regex aslo matches phone numbers in various formats, including those with international codes, area codes, and extension numbers.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Alternation](#alternation)
- [Escaping Characters](#escaping-characters)

## Regex Components

### Anchors

Anchors are used to match patterns at the beginning or end of a line. The `^` symbol at the beginning of our regex matches the start of a line, and the `$` symbol at the end matches the end of a line.
/^...$/



### Quantifiers

Quantifiers are used to specify the number of times a character or group should be matched. In our regex, we use `{1,3}` to specify that the preceding character or group should be matched between 1 and 3 times, and `?` to specify that it may or may not appear.



### Character Classes

Character classes are used to match any character within a specified set. In our regex, we use the character classes `\d` to match any digit, and `[-.()]` to match common phone number separators.

### Grouping and Capturing

Groups are used to capture a specific portion of a matched pattern. In our regex, we use four groups to capture the country code (if present), area code (if present), prefix, and line number separately.

