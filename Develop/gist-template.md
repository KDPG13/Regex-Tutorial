# Tutorial: Regex matching Hex value

Regular expressions are a sequence of characters that defines a search pattern for text. It is also defined as a string of text that allows you to create patterns to help with managing, matching, and locating text.


-Fun fact: regex come from the mathematical concept of regular sets.

## Summary

I will be discussing the parts of a regular expression that is used to match hex values. Any precise color can be accurately described to a computer using the hexadecimal scheme, ensuring consistency and accuracy in an electronic display. A six-digit number preceded by the # symbol defines a color that is utilized in a website or computer software. This code is known as a hexadecimal color value.  /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

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

Regular expressions give specific significance to anchors. They don't fit any of the characters. Instead, they align with a character's location before or after another:
The ^ anchor lines up with the start of the text.
The dollar sign ($) anchor corresponds to the end of the text.
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/

### Quantifiers
Regex quantifiers indicate how many times a character should be matched against. The ",+,?,{}" characters found within regulr expressions are regarded as quantifiers. The ? character describes that an expression occurs once or not at all. The * character describes that an expression occurs zero or more times. The + charcter defines that the expresion occures one or more times. The {n} charcter means that the expression occurs n or more times times and so on and so forth. Looking at our hex value, the numbers {6} and {3} in our Hex Value regular expression indicate that the component preceding these quantifiers should have a length of 6 for {6} and 3 for {3}.
### OR Operator
The | element in a regular expression defines the "or" operator. The or operator implies that it might be either of the components that we are separating with the |. When we look at our hex value, /^#?([a-f0-9]{6}  |  [a-f0-9]{3})$/, we see two compnents after the or operator. As a result, our hex value may either be 3 [a-f0-9]{3} or 6 characters ([a-f0-9]{6}.
### Character Classes
A group of characters surrounded in square brackets is referred to as a character class in the context of regular expressions. Looking at our hex value, our character are onside brackets. There are also two character classes; [a-f0-9] and [a-f0-9]. A-F looks for letters, while 0-9 looks for digits 0 to 9.

### Bracket Expressions
Brackets indicate a set of characters to match. Any individual character between the brackets will match, and you can also use a hyphen to define a set.
### Greedy and Lazy Match
A greedy match will try to match the longest possible string while a lazy <?> match will try to mach the smallest possible string. In our expression we have a lazy match. /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

## Author

Hello my name is Abdullahi Nur. I'm a full-stack developer student looking to futher succeed in this field.
Github: https://github.com/KDPG13/
