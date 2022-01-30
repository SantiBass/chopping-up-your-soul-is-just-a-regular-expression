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
Or oppretators
- #### 


/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)$/
### Character Classes
/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)$/
### Flags
/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)$/
### Grouping and Capturing
/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)$/
### Bracket Expressions
/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)$/
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
