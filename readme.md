# Regex-Tutorial
This tutorial breaks down the regular expression of email validation. 

## Summary
```
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```


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

```/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/```

## Anchors

The characters ```^``` and ```$``` are both considered anchors.
The ```^``` character is used at the beginning to signify the start of a Regex string. While the ```$``` character, is used at the end to signifies the completion of the Regex.


## Quantifiers

```+``` — **Matches the pattern one or more times.**

Equivalent to ```{1,}```. For example, ```/a+/``` matches the "a" in "candy" and all the "a"'s in "caaaandy".

```{}``` — **Curly brackets can provide three different ways to set limits for a match:* ```{ n } || { n, } || { n, x }```

```{ n }``` — **Matches the pattern exactly n number of times.**	

For example, ```/a{2}/``` doesn't match the "a" in "candy", but it matches all of the "a"'s in "caandy", and the first two "a"'s in "caaandy".

```{ n, }``` — **Matches the pattern at least n number of times.**

For example, ```/a{2,}/``` doesn't match the "a" in "candy", but matches all of the a's in "caandy" and in "caaaaaaandy".

```{ n, x }``` — **Matches the pattern from a minimum of n number of times to a maximum of x number of times.**

For example, ```/a{1,3}/``` matches nothing in "cndy", the "a" in "candy", the two "a"'s in "caandy", and the first three "a"'s in "caaaaaaandy". Notice that when matching "caaaaaaandy", the match is "aaa", even though the original string had more "a"s in it.

---

## Grouping Constructs

```()``` - **Way to group a section of Regex**

What is inside the ```()``` is known as a sub-expression. Capturing groups matches the match character sequence for possible reuse. 

## Bracket Expressions

```[]``` - **Anything inside ```[]``` represents a range of characters that we want to match.**

Example, ```[a-z]``` Includes all lowercase letter a-z. ```[0-9]``` Includes all numbers 0-9. ```[_-]``` Includes both _ and -


## Character Classes

**Character Class defines a set of characters.**<br>
```.``` - Find a single character, except newline or line terminator <br>
```\d``` - Find a digit<br>


## The OR Operator
```|``` -  Can provide as many terms as desired, as long as they are separated with the pipe character.

Example: ^I like ```(dogs|penguins)```, but not ```(lions|tigers)```$





## Sources
source - https://coding-boot-camp.github.io/full-stack/computer-science/regex-tutorial <br>
source - https://developer.mozilla.org/ <br>
source - http://web.mit.edu/gnu/doc/html/regex_3.html

## Author
Mikey Thompson<br>
### github https://github.com/methom21