# 
# Somraj RegEx Tutoral - URL with Regular Expression

URL Regex: A regular or rational expression defined as characters in a pattern or a sequence that replace or find string operations which may be useful locating a string in a URL.

## Summary
Regular expressions (regex or regexp) are extremely useful in extracting information from any text by searching for one or more matches of a specific search pattern (i.e. a specific sequence of ASCII or unicode characters).
Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

A Regex proves useful in matching a URL in order to locate special text patterns.

Matching a URL: `/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/`
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
Matching a URL: `/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/`

### Anchors
Anchors don't actually stand for any specific character in the regex. Anchors show where the text starts and ends in the expression. For URL RegEx, it has two anchors: ^ and $
- "^" Caret anchor marks the beginning of the regular expression text which can be found near the start of the expression. 
- "$" Dollar sign anchor can be found at the end of the expression and represents end of the text.
### Quantifiers

### Grouping Constructs

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags
Regular expressions can have flags that affect the search. For this specific regex the following flags will be important the mutli line flag and the global flag. The global flag return all matches. Without this flag it would only return the first line that matched the regex, which wouldn't be an issue if we were checking one URL at a time but that isn't very efficient.

- i: Ignores casing. Makes expression case-sensitive
- g: Global. Makes expression search for all occurences
- s: Dot All. Makes the wild characters . match newlines as well
- m: Multiline. Makes boudnary characters ^ and $ match beginning and end of every line.
- y: Sticky. Indicates that it matches only from the index indicated by the lastIndex property of this regular expression in the target string (and does not attempt to match from any later indexes)
- u: Unicode. Expression assumes individual characters are code points, not code units and will then match 32 bit characters.

### Character Escapes

## Author

Parankush Somraj is SAP Analyst working for financial data provider company in Manahattan, NY and also currently enrolled in Rutgers Coding Bootcamp in pursuit to become a full stack software developer

Fun Facts:
- I enjoy running outdoors in the winter - Checkout contact section below about my running profile
- IPA Craft Beers from Treehouse are my favorites. We made a trip to visit Santa Rosa for Russian River and stood in line for 4 hours to get 2 west coast style IPAs

* [Parankush Somraj's Github](https://github.com/bootcamparankush)  
* [Parankush Somraj's LinkedIn](https://www.linkedin.com/in/parankush-somraj-6b372b1/)
* [Parankush Somraj's Email](mailto:parankush.somraj@gmail.com)
