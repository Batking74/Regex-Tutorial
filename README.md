# Phone Number and Email Regular Expression Totorial

Welcome to the "Phone Number and Email Regular Expression Tutorial"! In this guide, we will delve into the fascinating world of regular expressions (regex) specifically tailored for validating and extracting phone numbers and email addresses. Regular expressions are powerful tools used in programming and data validation, enabling developers to define patterns for matching and manipulating text efficiently. Whether you're a beginner looking to understand the fundamentals or an experienced coder aiming to refine your skills, this tutorial will provide you with insights and practical examples to master regex patterns for phone numbers and email addresses. Let's embark on a journey to demystify these essential patterns and enhance your proficiency in handling contact information within your applications.




## Summary
In this tutorial, we'll cover regular expressions for validating both phone numbers and email addresses. The regex for the phone number, as mentioned earlier, ensures the format (XXX) XXX-XXXX, where X represents a digit. The regex for the Email address, ensures the format example@gmail.com, where 'example' is the name of the email. Listed below are examples of these regex's:
```bash
# Phone Number Regex
^\(\d{3}\) \d{3}-\d{4}$

# Email Address Regex
^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$
```



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
- What are Regex Components? Regular expressions (regex) consist of various components that define patterns for matching strings. Here are some fundamental components commonly used in regex:

## Anchors (^ and $)
- `^`: Asserts the start of a line.
- `$`: Asserts the end of a line.

**Example (Phone Number):**
- Valid: `^(123) 456-7890`
  - Regex Syntax: `^\(\d{3}\) \d{3}-\d{4}$`
- Invalid: `123 456-7890` (doesn't start with `()`)
  - Regex Syntax: N/A (Anchors are not relevant for this invalid case)

**Example (Email Address):**
- Valid: `user@example.com`
  - Regex Syntax: N/A (Anchors are not used for email validation)
- Invalid: N/A (Anchors are not used for email validation)
  - Regex Syntax: N/A (Anchors are not used for email validation)

## Quantifiers (*, +, ?, {n}, {n,}, {n,m})
- `*`: Matches 0 or more occurrences.
- `+`: Matches 1 or more occurrences.
- `?`: Matches 0 or 1 occurrence.
- `{n}`: Matches exactly n occurrences.
- `{n,}`: Matches n or more occurrences.
- `{n,m}`: Matches between n and m occurrences.

**Example (Phone Number):**
- Valid: `^(123) 456-7890`
  - Regex Syntax: `^\(\d{3}\) \d{3}-\d{4}$`
- Invalid: `^(123) 456--7890` (more than one hyphen in the local code)
  - Regex Syntax: `^\(\d{3}\) \d{3}-\d{4}$`

**Example (Email Address):**
- Valid: `user@example.com`
  - Regex Syntax: `^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$`
- Invalid: `user@@example.com` (more than one @ symbol)
  - Regex Syntax: `^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$`

## Grouping Constructs ( )
- `( )` are used to create a group for the area code.

**Example (Phone Number):**
- Valid: `^(123) 456-7890`
  - Regex Syntax: `^\(\d{3}\) \d{3}-\d{4}$`
- Invalid: `(123 456-7890`
  - Regex Syntax: N/A (Invalid example, doesn't follow regex structure)

**Example (Email Address):**
- Valid: `user@example.com`
  - Regex Syntax: `^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$`
- Invalid: `user@exam ple.com` (contains a space)
  - Regex Syntax: N/A (Invalid example, doesn't follow regex structure)

## Bracket Expressions ([ ])
- Define a character class, matching any one of the characters within the brackets. For example, `[aeiou]` matches any vowel.

**Example (Phone Number):**
- Valid: `^(123) 456-7890`
  - Regex Syntax: N/A (Not applicable to the phone number pattern)
  
**Example (Email Address):**
- Valid: `user@example.com`
  - Regex Syntax: `^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$`
- Invalid: `user@example[dot]com` (contains special characters within brackets)
  - Regex Syntax: `^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$`

## The OR Operator (|)
- The OR operator is represented by `|` and allows for alternative matches. For example, `cat|dog` matches either "cat" or "dog".

## Flags (i, g, m)
- Flags are used to modify the behavior of the regex.
  - `i`: Case-insensitive matching.
  - `g`: Global matching (find all matches).
  - `m`: Multi-line matching.

**Example (Phone Number):**
- Valid: `^(123) 456-7890`
  - Regex Syntax: N/A (Not applicable to the phone number pattern)
  
**Example (Email Address):**
- Valid: `user@example.com`
  - Regex Syntax: `^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$`

## Character Escapes (\)
- `\(` and `\)`: Escape characters for literal parentheses.

**Example (Phone Number):**
- Valid: `^(123) 456-7890`
  - Regex Syntax: `^\(\d{3}\) \d{3}-\d{4}$`
- Invalid: `123 456-7890` (without escaped parentheses)
  - Regex Syntax: N/A (Invalid example, doesn't follow regex structure)

**Example (Email Address):**
- Valid: `user@example.com`
  - Regex Syntax: `^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$`
- Invalid: `user@example!com` (without escaping the dot)
  - Regex Syntax: N/A (Invalid example, doesn't follow regex structure)


## Author
As a passionate FullStack developer, my devotion to technology is at the core of who I am. Embracing a self-taught journey, I thrive on continuous learning and sharing knowledge. My commitment to the ever-evolving tech landscape goes beyond coding; it's about innovative problem-solving and contributing a unique perspective to every project. Whether crafting robust code or collaborating on diverse tech endeavors, I bring a blend of expertise and a love for self-directed learning to create impactful solutions.

GitHub: https://github.com/Batking74
