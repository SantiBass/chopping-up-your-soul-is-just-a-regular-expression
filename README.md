# This is a Regex Tutorial
Introductory paragraph (replace this with your text)

### As part of my journey to become a web developer, I have created a tutorial in which I explain the use for regular expressions aka "Regex". This tutorial will help us understand search patterns implementing regex. 


## Summary
### Regex or "Regular Expression" is a tool that help us to define a search pattern. This expression is regularly a sequence of characters that would simplify our global search. At first sight, it seems very intimidating string of characters but after break it down to its most basic components, it will become more like a game for kids. So let's dive in! Let's take a look at this regex:
### /^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)$/
### To sail into our journey to understand this regex let's take a look at the "Table of Content"


## Table of Contents
### 
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
- #### `^` The caret anchor is used to mach any string at the beginning of a regex.
- #### `$` The dollar sign anchor is used to match the end of a string or a line before it in a regex. This matches a position, not a character.
    #### Here are some examples of anchors:
    #### `^(https://) = https;//` because the expression is within parenthesis.
    #### `(funny animals)$` = funny animals because the expression is within parentheses   

### Quantifiers
Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found in any regular expression.
- ####  `* `It matches a string that with `ab` followed by zero or more `c`. For example: abc* = (`abc`, `abc`ccc). But abc ≠ (acb, abbc aabbcc) etc.
- ####  `+ `It matches a string that with `ab` followed by zero or more `c`. For example: abc* = (abc, abcccc). But abc ≠ (acb, abbc aabbcc) etc.
- ####  `? `It matches one or zero occurrences of a character(s) on its left in a string. For example: `https? `will only match `https` once from `https`//
- ####  `{n} `It matches the first character once plus a specific `'nth'` occurrence of the next character in a preceding string. For example: ab{3} will only match `abbb` from `abbb`bca, aa`abbb`b etc.
- ####  `{n,} `It matches the first character once plus the next character form `'nth'` times in a preceding string. For example: ab{2,} will match `'a' `and as many `'b'` from `abbbbbb`bca, aa`abbbbbbbbbb` etc.
- ####  `{n,m} `It matches between `'min'` to `'max'` occurrences of characters on its preceding string. For example ([a-z\.]{2,6}) = `ab`23ab, `abcdge`gegege, 123`asdd`, etc 
- #### A regular expression follow del

### OR Operator
OR operators, also known as Alternation Operator, act like a boolean operator. Les's take a look to a couple examples of the 'OR' operator.

- #### `|` this `OR` operator matches the outer string plus the character(s) before or after itself that are within the parenthesis. For example: `a(b|c)` will match `ab`c, `ac`b, or cool`ab`fan, etc, in a string.
- #### `[]` this `OR` operator matches the outer string plus one of the characters within the brackets. For example: `a[bc]` will match `ab`c, `ac`b, or cool`ab`fan, etc, in a string 


### Character Classes
Character classes, also known as `'Charcter Set'`, is used to match only one out of a set of specific characters. These characters can be digits, words, or white spaces.
- #### `\d ` It matches a single character from 0-9.  For example: `alpha34`, it will match `3` in alpha`3`4.
- #### `\D ` It matches a single character that is not a digit character from 0-9.  For example: `34aplha34`, it will only match `a` in 34`a`lpha34.
- #### `\w ` It matches a word character including alphanumeric and underscore. For example: `\w`  will match  `h` in   `h`i or `\w\w` will match `hi`.
- #### `\W ` It matches any character that is not a word character including alphanumeric and underscore.
- #### `\s ` It matches any whitespace character and that includes spaces, tabs, line breaks. For example ` `.
- #### `\S ` It matches any character that is not a whitespace character and that includes spaces, tabs, line breaks.
- #### `. ` It matches any character.
- #### ``
/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)$/
### Flags
Flags  are parameters that allow us to search for expressions in a different way. Each flag is made of a single character and have different functions. Here are some examples.

- #### `g` This flag is called Global flag. A global flag will match any character globally. For example: `/ll/g` will match `ll` form he`ll`o.
- #### `m` This flag is called Multiline flag. When the multiline flag is enabled, beginning and end anchors (^ and $) will match the start and end of a line, instead of the start and end of the whole string.
- #### `i` This is the Ignore Case flag. It makes the whole expression case-insensitive. For example, `/aBc/i` would match `AbC`.
/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)$/
### Grouping and Capturing
Grouping and Capturing allows us to make a string or a pattern a whole so it can be matched as a block.
- #### `() ` A pair of parenthesis creates a capture group.  For example: `(https)` creates a capturing group with a value of `https`
- #### `(?:) ` When we use `?:`, it groups multiple tokens together without creating a capture group. For example: `(https?:)` will match `https:`
- #### `(?<>) ` Creates a capturing group that can be referenced via the specified name. For example: `a(?:<fun>bc)` will match `abc` with the group name of fun.


### Bracket Expressions
Bracket Expressions are characters enclosed by a pair of bracket.
- #### `[]`. It will match any single character within the pair of brackets. For example: `[a-z]` will match any character from `a` to `z`.
- #### `[]%` It will mach any string within the brackets before the percent sign `%`. For example: `[abc]%` will match `c%` from ab`c%`.
- #### `[^]` It will match any character os string that has not a letter from within the brackets. This is a negation expression. For example: `[^a-z]` will not match any characters from `a-z` but will mach numbers.
*note: if the first character within the brackets is a `^` then it signifies any chracter **not** in the list, and is unspecified whether it matches an encoding error. 


### Greedy and Lazy Match



/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)$/
### Boundaries
/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)$/
### Back-references
/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)$/
### Look-ahead and Look-behind
/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)$/
## Author
/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)$/
A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
