# Title (Chelsea's Regex )

Introductory paragraph (replace this with your text)
A regular expression shortened as regex or regexp; sometimes referred to as rational expression is a sequence of characters that specifies a match pattern in text. Usually such patterns are used by string-searching algorithms for "find" or "find and replace" operations on strings, or for input validation. Regular expression techniques are developed in theoretical computer science and formal language theory.
## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.
Will be briefly describing the regex componets and squence and main elements. And a understanding of the Regex, and how the function to make elements comply, with the code given. The code snippet  // Example text
let text = "Hello, my email is Chelsea1983@gmail.com";

// Define the pattern
let pattern = /\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Za-z]{2,}\b/g;

// Find matches
let matches = text.match(pattern);

// Print the matches
for (let i = 0; i < matches.length; i++) {
  console.log(matches[i]);
}

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
let text = "Hello world, welcome to the testing site";
console.log(/^Hello/.test(text)); // true
console.log(/site$/.test(text)); // true
console.log(/\bwelcome\b/.test(text)); // true
console.log(/\Btesting\B/.test(text)); // true


### Quantifiers
let text = "aaabbbccc";
console.log(/a+/g.exec(text)); // ["aaa"]
console.log(/a+?/g.exec(text)); // ["a"]
console.log(/b{2}/g.exec(text)); // ["bb"]
console.log(/b{2,4}/g.exec(text)); // ["bbb"]


### OR Operator
let text = "Hello, world!";
console.log(/Hello|world/.test(text)); // true
console.log(/Hi|world/.test(text)); // true
console.log(/Hi|universe/.test(text)); // false
In this example, we have a string text that contains the phrase "Hello, world!". We use the OR operator (|) to define alternative patterns.

/Hello|world/ matches if either "Hello" or "world" is found in the text, which is true.
/Hi|world/ matches if either "Hi" or "world" is found in the text, which is true.
/Hi|universe/ matches if either "Hi" or "universe" is found in the text, which is false because neither "Hi" nor "universe" is present.
Note that the OR operator matches the first alternative it finds. If multiple alternatives are valid at a given position, the first one encountered will be chosen.

The OR operator can be combined with other regular expression elements, such as quantifiers or capturing groups, to create more complex patterns that allow for flexible matching in your regular expressions.








### Character Classes
[0-9]: Matches any single digit from 0 to 9.

Example: /[0-5]/ matches any digit from 0 to 5

### Flags
g (global): Matches all occurrences of the pattern in the input string, not just the first one.

### Grouping and Capturing
let text = "aaaaab";
let pattern = /(a+)/;
let match = pattern.exec(text);

console.log(match[1]); // "aaaaa"


### Bracket Expressions

/[^0-9]/
### Greedy and Lazy Match
(/a.*b/) the Greedy match and lazy /a.*?b/
### Boundarieshbu \\\\\\\\\\\-
/abc$/ matches "abc
### Back-references

### Look-ahead and Look-behind
 ((?=...), (?!...)) and 
## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
