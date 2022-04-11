Regex Tutorial

In this Regex (Regualar Expression) tutorial you will get information that will help you understand how it works when matching email. To get a valid email id you use a regular expression.The reasons for validating email addresses; one is to improve usability. The second is to make sure that noone enters a dummy addresses. 

## Summary

s a sequence of characters that defines a specific search pattern. When included in code or search algorithms, regular expressions can be used to find certain patterns of characters within a string, or to find and replace a character or sequence of characters within a string. They are also frequently used to validate input.This tutorial will cover how its used to match email. 
Matching an Email: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
## Table of Contents

- [Anchors](#anchors)
- [Greedy Quantifiers](#Greedy-Quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

Regex Components
### Anchors
Matching an Email: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
He we will start with anchors component. The anchors used for matching an email are ^ which shows the start of the string. The end of the string can be indicated with $.

### Greedy Quantifiers
Matching an Email: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
Repeats the previous item once or more. Greedy, so as many items as possible will be matched before trying permutations with less matches of the preceding item, up to the point where the preceding item is matched only once.

### Character Classes
Matching an Email: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
For the character class in this expression is \d, which matches a single characters that is a digit from 0-9. A good thing to note is it will only match a single digit like "2", but not "55".

### Grouping Constructs
Matching an Email: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
There are part of the capturing group. The first Capturing group in the expression is ([a-z0-9_\.-]+) which matches the users email name. The second capturing group is ([\da-z\.-]+) which will match the email service. The last capture group is ([a-z\.]{2,6}) to capture the domain.

### Bracket Expressions
Matching an Email: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
Bracked expressions for email validation includes the character sets of [a-z0-9_\.-], which is matching any letter a-z and is case senstive. It also matches a character 0-9 and matches the characters "_" , "-" , and "."; [\da-z\.-], which is matching a single digit from 0-9, any character a-z (case senstive), and the characters "." and "-".; [a-z\.] matches any character a-z(case senstive) and the character ".".

### Character Classes
Matching an Email: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
The character class is the most basic regex concept after a literal match. It makes one small sequence of characters match a larger set of characters. For example, [A-Z] could stand for any uppercase letter in the English alphabet, and \d could mean any digit.
### The OR Operator
Matching an Email: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
The "or" operator is defined using the | element. 

### Flags
Matching an Email: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
Regular expressions have optional flags that allow for functionality like global searching and case-insensitive searching. These flags can be used separately or together in any order, and are included as part of the regular expression.
These flags include g , i , m , u , s , y all will different meaning.

### Character Escapes
Matching an Email: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
Lastly the \ is known as the escape code, which restores the original literal meaning of the following character. Similarly, *, +, ? (occurrence indicators), ^, $ (position anchors) have special meaning in regex. You need to use an escape code to match with these characters.

Author
https://github.com/CalvinTurner10