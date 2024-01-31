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
### What are Regex Components?
Regular expressions (regex) consist of various components that define patterns for matching strings. Here are some fundamental components commonly used in regex:



### Anchors
Anchors are used to assert positions in the string. Commonly used anchors include:
- ^ (caret): Asserts the start of a line.
- $ (dollar sign): Asserts the end of a line.

### Quantifiers
Quantifiers specify the number of occurrences of a character or group. Common quantifiers include:
- * (asterisk): Matches 0 or more occurrences.
- + (plus): Matches 1 or more occurrences.
- ? (question mark): Matches 0 or 1 occurrence.
- {n}: Matches exactly n occurrences.
- {n,}: Matches n or more occurrences.
- {n,m}: Matches between n and m occurrences.

### Grouping Constructs
Grouping constructs are used to create subexpressions or capture groups. They are enclosed in parentheses ( ).

### Bracket Expressions
Bracket expressions define a character class, matching any one of the characters within the brackets. For example, [aeiou] matches any vowel.

### Character Classes
Character classes match a single character from a set of characters. Common character classes include:

- \d: Matches any digit (equivalent to [0-9]).
- \w: Matches any word character (alphanumeric + underscore).
- \s: Matches any whitespace character (space, tab, newline).

### The OR Operator
The OR operator is represented by | and allows for alternative matches. For example, cat|dog matches either "cat" or "dog".

### Flags
Flags are used to modify the behavior of the regex. Common flags include:

- i: Case-insensitive matching.
- g: Global matching (find all matches).
- m: Multi-line matching.

### Character Escapes
Some characters have special meanings in regex and need to be escaped with a backslash \ to be treated literally. For example, \. matches a literal dot.

## Author
As a passionate FullStack developer, my devotion to technology is at the core of who I am. Embracing a self-taught journey, I thrive on continuous learning and sharing knowledge. My commitment to the ever-evolving tech landscape goes beyond coding; it's about innovative problem-solving and contributing a unique perspective to every project. Whether crafting robust code or collaborating on diverse tech endeavors, I bring a blend of expertise and a love for self-directed learning to create impactful solutions.

GitHub: https://github.com/Batking74