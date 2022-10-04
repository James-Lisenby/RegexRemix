Homework challenge 17: Email Regex Tutorial

Being a well equipped developer is more then just writing the code. A good deveolper also writes about the code! In this tutorial I will be explaining how a Regex, or regular expression can be used to match an email.

## Summary

In this tutorial we will take a look at an example of a Regex, or regular expression. What is a regex you might ask? Well, a regex is a set of characters that defines a search pattern within text. This can be used to find things like emails, usernames, URL's, or HTML tags to name a few. In this specific article I will be going over how we can use a regex to match emails and how the expression breaks up the characters.

Matching an Email: /^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/

To start, a regex as an literal expression, is wrapped in forward slashes(/) at the start and the end of the expression. Inside the forward slashes are additional components. They are as follows: Anchors, quantifiers, grouping constructs, bracket expressions, character classes, OR operators, flags, and character escapes.

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

^ and $ are the anchors. Theese characters are used to mark the start and the end of the string inside the expression.

### Quantifiers

Theese are the numbers between the two sets of curly brackets near the end of the regex. In our example you see the number 2 and 6. This states that each section of the string is a minimumn of 2 characters and a max of 6.

### Grouping Constructs

Expressions are usually broken up into sections using (). The groups in this example are of the capture category, meaning the save matched sequeneces for reuse. Using our example above, notice that the expression is broken into 3 seperate sections. Inside of each section is a set of [] with characters inside. Theese are the ....

### Bracket Expressions

...Bracket Expressions! The purpose of the bracket expressions is too create a range of characters that tell us what we want to match within the text. In our example you see 3 different sections.

[0-9] denotes any number between 0 and 9. [a-z] denotes any lowercase leter from a to z. If you wanted to also include uppercase letters, you would need to use [a-zA-Z]. Lastly, [.-] denotes the special characters that can be used: underscore (), backwards slash (/), period (.), and dash (-).

### Character Classes

A character class can define a set of characters that can occur in input strings to fullfill a match. The bracket expressions mentioned previously are examples of this. There are two more examples that can be found in our email example.

A period (.) matches any character except the newline character (\n).

(\d) denotes any Arabic number and is equal to the bracket expression [0-9].

### Character Escapes

The last component we will look at are character escapes. A character escape uses a backslash to force a regex to look at the character following the backslash instead of using it in a literal. In our example above, you can find one example, (.). This denotes that we want the expressiion to look directly for a period (.) instead of the character class using the same symbol.

### Sources

https://www.youtube.com/watch?v=7DG3kCDx53c
Video - Intro to Regex

https://coding-boot-camp.github.io/full-stack/computer-science/regex-tutorial
The full-stack blog
