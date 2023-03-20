# Regex Review - Email

Regex patterns are coded patterns used to describe a set of strings that match the given pattern. Today, we will be reviewing the different components of the regex patterns.

## Summary

We will be reviewing the regex pattern that is used to match/reject an email address and how each component functions in the code.

Example: 

let email =  /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Table of Contents

- [Regex Review - Email](#regex-review---email)
  - [Summary](#summary)
  - [Table of Contents](#table-of-contents)
  - [Regex Components](#regex-components)
    - [Anchors](#anchors)
    - [Quantifiers](#quantifiers)
    - [Grouping Constructs](#grouping-constructs)
    - [Bracket Expressions](#bracket-expressions)
    - [Character Classes](#character-classes)
    - [Character Escapes](#character-escapes)
  - [Author](#author)

## Regex Components

let email =  /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

### Anchors

^ and $

The first component of the regex expression we will be dicussing are the anchors. The anchors will mark the beggining and the ending of the string/ expression of the regex expression.
The anchors in this regex expression are ^ and $. The ^ will signal the beginning of the regex expression while the & will signal the end of the regex expression.

### Quantifiers
+ and {2,6}

The quantifiers are used to communicate with the expression as to how many characters are expected in the string. In this expression, the quantifiers are +, {2,6}. The + in this expression is going to connect the email with the email service provider. the {2,6} in this expression is going to allow input with characters between 2 and 6 only allowing the character set of [a-z\.]. This will allow any alphabetic letter into the string along with a period.

for example, the quantifier of + will allow the connection of email + email service used + .com (khernandez0810 + @ + gmail +.com)

### Grouping Constructs
[]

The grouping construct is going to signla the expression to group the characters within the parenthesis. In the email example, the grouping construct is using thje parentheses. In the email expression, the grouping used is ([a-z0-9_\.-]+), ([\da-z\.-]+) and ([a-z\.]{2,6})$/. each grouped parenthesis will be 3 seperate groups of characters connected by the quantifier "+" to connect them.

### Bracket Expressions
[a-z0-9_\.-], [\da-z\.-], [a-z\.]. [a-z0-9_\.-]

The bracket expressions are used to group the characters given the character sets allowed in the expression. Each bracket expression  In ther email example, the bracket expressions are [a-z0-9_\.-], [\da-z\.-], [a-z\.]. [a-z0-9_\.-] will allow alphabetical characters (a-z), numerical characters (0-9), and will allow the symbol of ., _ and -. The second bracket expression is [\da-z\.-]. \d will allow for any digit, a-z will allow for an alphabetical character (a-z) and finally will allow input of the special characters . -, and _ .  The third bracket expression is [a-z\.]. This will allow any alphabetic letter into the string along with a period.

### Character Classes
\d

The character classes are used to define a set of characters. In this email example, the character class used is "\d". The \d will allow any numerical digit. It can also be used as [0-9].


### Character Escapes
\.

The character escape used in the email regex is the \. using the backslash in front of the period will cause the period to act as literal instead of making it a special character.

## Author
Kevin Hernandez

My name is Kevin Hernandez and you can view my projects at http://github.com/khernandez0810
