
## Somraj RegEx Tutoral - URL with Regular Expression

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
- [Author](#author)
- [Credits](#credits)

## Regex Components
Matching a URL: `/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/`

### Anchors
Anchors don't actually stand for any specific character in the regex. Anchors show where the text starts and ends in the expression. For URL RegEx, it has two anchors: ^ and $
- "^" Caret anchor marks the beginning of the regular expression text which can be found near the start of the expression. 
- "$" Dollar sign anchor can be found at the end of the expression and represents end of the text.

### Quantifiers
Quantifiers will measure and set the limit on the the number of characters that we are wanting to match in our Regex: ```+``` searches the pattern one or more times, ```?``` searches the pattern zero or one time, * searches the pattern zero or more times.
``` https? ``` for= example. The ? will make the preceeding itme optional.

### Grouping Constructs
Grouping Construct is a part of a pattern that can be enclosed in a parentheses () and is a way to treat multiple characters as one unit. The example expression has many groupings such as: 
```https?:\/\/``` which is looking for the http(s),```(www\.)?[\d-a-zA-Z0-9@:%._\+~#=]``` which will look for initial domain, ```[a-zA-Z0-9()]{1,6}\b([-a-zA-Z0-9()@:%_\+.~#?&//=]``` looks for top level domain, and ```*)``` file paths.

### Bracket Expressions
Bracket Expression is a matching or non-matching list expression and consists of one or more expressions that will be found in square brackets []. It represents a special character class and is a quantified rule providing range construct. They adapt to a users or applications locale. 

### Character Classes
A character class is  the set of characters that could occur in a string.  
The \d character class in the above code is looking for any digits, whereas a \D looks for non-digits, \s searches for space symbols, tab and newlines, \S looks for all but \s, \. any characters with the regex 's' flag, while the included \w character is looking for an alphanumeric character. 

### The OR Operator
In regular expressions, the OR operator is represented by the pipe character '|'
The purpose of an OR operator is to match the characters on the left or right of the operator, essentially serving as an or, as in and/or. Using the | as in m|M would match either m or an M from the string. If we had used ```https?:\/\/(www\.)?[\d-a|A``` it would search or a OR A.

### Flags
Regular expressions can have flags that affect the search. For this specific regex the following flags will be important the mutli line flag and the global flag. The global flag return all matches. Without this flag it would only return the first line that matched the regex, which wouldn't be an issue if we were checking one URL at a time but that isn't very efficient.

- i: Ignores casing. Makes expression case-sensitive
- g: Global. Makes expression search for all occurences
- s: Dot All. Makes the wild characters . match newlines as well
- m: Multiline. Makes boudnary characters ^ and $ match beginning and end of every line.
- y: Sticky. Indicates that it matches only from the index indicated by the lastIndex property of this regular expression in the target string (and does not attempt to match from any later indexes)
- u: Unicode. Expression assumes individual characters are code points, not code units and will then match 32 bit characters.

### Character Escapes
 Character escapes are used to represent special characters or character classes. Some commonly used character escapes for regex 
- \d - matches any digit (0-9)
- \w - matches any word character (alphanumeric and underscore)
- \s - matches any whitespace character (space, tab, newline)
- \D - matches any non-digit character
- \W - matches any non-word character
- \S - matches any non-whitespace character

## Author
Parankush Somraj is SAP Analyst working for financial data provider company in Manahattan, NY and also currently enrolled in Rutgers Coding Bootcamp in pursuit to become a full stack software developer

Fun Facts:
- I enjoy running outdoors in the winter - Checkout contact section below about my running profile
- IPA Craft Beers from Treehouse are my favorites. We made a trip to visit Santa Rosa for Russian River and stood in line for 4 hours to get 2 west coast style IPAs

* [Parankush Somraj's Github](https://github.com/bootcamparankush)  
* [Parankush Somraj's LinkedIn](https://www.linkedin.com/in/parankush-somraj-6b372b1/)
* [Parankush Somraj's Email](mailto:parankush.somraj@gmail.com)

## Credits

* [Regex tutorial — A quick cheatsheet by examples](https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285)
