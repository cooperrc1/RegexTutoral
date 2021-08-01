# Regex Tutorial

Welcome to a quick tutorial displaying how Regex works

## Regex is short for regular expression! Its a string which you can use to manage, match, and find text.
Here is a line of Regex which is used to match a Hex Value: /^#?([a-f0-9]{6}|[a-f0-9]{3})$/



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
Used to match strings that begin or end with a certain character.
These are some examples of Anchors ^ - Start of string or line $ - End of string or line.
### Quantifiers
Specifies how many instances of a group, character, or character class must be in the input for a match to be found.
These are some examples of Quantifiers /X./; // matches any character /X*/; // Matches zero or several repetitions of letter X, is short for {0,} /X+-/; // matches one or more repetitions of letter X, is short for {1,} /X?/; // finds no or exactly one letter X, is short for is short for {0,1}. // d{3}; // matches three digits. {} describes the order of the preceding liberal // d{1,4} ; // means d must occur at least once and at a maximum of four
### OR Operator
Splits the text with a bar and matches everything to the left or right of the bar. If you want to limit the reach of it you need parenthesis, mostly used with booleans.
These are some examples of OR Operators

(some truthy expression) || expr expr1 || expr2
### Character Classes
Used to tell the regex engine to match only one out of several characters
These are some examples of Character Classes

\d - any single digit 0-9 \w - a word character \s - spaces, tabs \t, new lines \n and a few other rare characters such as \v, \f, \r.

\D - Any character except \d \W - Anything but \w \S - Any character except \s

. - Any character if with the regexp 's' flag, otherwise any except a newline \n.
### Flags
Regex have six optional flags that allow for functionality like global and case insensitive searching. These flags can be used separately or together in any order, and are included as part of the regular expression.
These are some examples of flags. d - Generates indices for substring matches. g - Global search. i - Case-insensitive search m - multi-line search s - Allows . to match newline characters. u - "unicode"; treat a pattern as a sequence of unicode code points. y - Perform a "sticky" search that matches starting at the current position in the target string.

Grouping and Capturing
### Grouping and Capturing
Pattern or string that is matched in a complete book.

These are some examples of Grouping and Capturing
() - Creates a capture group (?:) - disables the capturing group (?<>) - puts a name to the group
### Bracket Expressions
Match one character out of a set of characters, just like regular character classes.
These are some examples of Bracket Expressions. [] - matches any single character within the brackets []% - matches the string inside the brackets before the % [^] - matches any string that has not a letter from within the brackets (negation of expression)
### Greedy and Lazy Match
Expand the match as far as possible through the text.
These are some examples of Greedy and Lazy Matching. * + {} - These characters can be used as a quantifier for Greedy or Lazy match.
### Boundaries
These are the places between characters. Boundaries should be thought of as a wall between characters. There are two types, you have WORD and NON-WORD.
These are some examples of Boundaries \b - Position that bounds a word. \B - Exact opposite of \b \* - Match between a word and word character, as well as non word and non word character
### Back-references
Reference of a captured match, saved in memory, by a captured group.

These are some examples of Back references. ([xyz])\1 using \1 it matches the same text that was matched by the first capturing group ([uwx])([yz])\2\1 we can use \2 (\3, \4, etc.) to identify the same text that was matched by the second (third, fourth, etc.) capturing group (?[xzy])\k we put the name bar to the group and we reference it later (\k). The result is the same of the first regex
### Look-ahead and Look-behind
Lookahead and lookbehind, collectively called “lookaround”, are Zero-length assertions just like the start and end of line. The difference is that lookaround actually matches characters, but then gives up the match. Returning only the result match or no match. That is why they are called assertions.

These are some examples of Look around.

h(?=t) - a h only if is followed by t, but t will not be part of the match (?<=t)h - a h only if is preceded by a t, but t will not be part of the match

h(?!t) - a h only if is not followed by t, but t will not be part of the match (?<!t)h - a h only if is not preceded by a t, but t will not be part of the match
## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
I'm Cooper and I am 19, here's my github. https://github.com/cooperrc1
