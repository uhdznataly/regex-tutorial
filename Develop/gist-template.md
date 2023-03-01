
# Regex Tutorial: Matching a URL

This tutorial will explain the use of regex to "matching an email" using the expression "/^([a-z0-9_\.-]+)@([\da-z\.-]+)/.([a-z\.]{2,6})$/".

# Summary

 The definition of a regular expression, or Regex, is a sequence of symbols and characters expressing a string or pattern to be searched for within a longer piece of text. Because of this, we are able to take these expressions and match them to things like an email, URL, or HTML tag. This specific tutorial will go through the components of a regex and how it applies to an email.    

## Table of Contents

* [anchors](#anchors)
* [quantifiers](#quantifiers)
* [groupingconstructs](#groupingconstructs)
* [bracketexpressions](#bracketexpressions)
* [characterclasses](#characterclasses)
* [theoroperator](#theORoperator)
* [flags](#flags)
* [characterescapes](#characterescapes)


## Anchors

In a regex for matching an email, anchors are used to specify the beginning and end of an input string. The caret (`^`) anchor is used to indicate the beginning of the string. The dollar sign (`$`) anchor is used to indicate the end of the string. These are both used to ensure that the regex matches only the email address and not any other text that may appear before or after it. Therefore, the regex will only match to the email and nothing else.  


## Quantifiers

Quantifiers are used to specify the number of times a particular character or group of characters should be matched in the input string. There are many type of quantifiers that an be used to match an email. For example, we have the plus sign (`+`). This will connect the users email name + domain (ex: yahoo.com). The curly braces (`{}`) are another type of quantifier. If for example, we had the quantifier of {3, 9}, this would match anything between 3 and 9 characters long for the character set. The user can combine different type of quantifiers with other regex syntax to create more complex patterns for matching an email.  


## Grouping Constructs


Grouping constructs in regex of matching an email can be used to match specific parts of an email address and extract them as seperate entities. In the string `([a-zA-Z0-9._%+-]+)` for example, matches one or more characters that are alphanumeric or has any of the following special characteristics: underscore (`_`), dot (`.`), percent (`%`), or hyphen (`-`). This string means the group must end with a dot followed by two or more charcteristics that are alphabetic. 


## Bracket Expressions


Bracket expressions are a list of characters and/or character classes enclosed in brackets. They are used in regex to match a set of characters within a given range. Yoy can use the following pattern: `^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$` to match an email address. For example, `[a-zA-Z]{2,}$` will match two or more occurences of alphabetic characters that represent the top-level domain.  
 

## Charcter Classes


Character classes allow a used to define a set of characters that can match a specific pattern to in the email address. An example of a character class is the string: `[a-zA-Z0-9._%+-]`. This will match any alpahnumeric character, including special characters commonly found in email addresses. Overall, character classes allow the user to specify a range of characters that can be matched, which helps to create more flexible and accurate regex patterns for matching email addresses


## The OR Operator


The OR operator in regex is denoted by the pipe symbol (`|`). It allows the user to match either one pattern or another. In the regex `^[a-zA-Z0-9._%+-]+@(?:[a-zA-Z0-9-]+\.)+[a-zA-Z]{2,}$`, it will match email addresses that start with one or more alphanumeric characters follow by the At (`@`) symbol and then the domain name. The domain name can be either a series of alphanumeric characters separated by hyphens, followed by a period and a top-level domain (TLD) such as (`.com`) or (`.net`), or it can be a single word TLD like (`.edu`) or (`.gov`).


## Flags


Flags in a rwgualr expression are used to modify how the regex pattern is interpreted and matched again text. For example, the case-insensitive flag (`i`) makes the pattern macth case-insensitively. It's commonly used in email regex because email addresses are not case-sensitive. Another example is the multiline flag (`m`). This will pattern match across multiple lines. It can be useful if a user is trying to match an email address that spans multiple lines in a larger text.


## Character Escapes


Character escapes are used in regex to match specific characters or character squences that have special meaning in regen syntax. The backlash escape is used to escape special characters that have a specific meaning in regular syntax. For example, using `\s` matches a chacater that is either a whitespace or non-whitespace chacater. 


# Author


Written by Nataly Rodriguez.
Contact using-
Email: uhdznataly@yahoo.com
Github: https://github.com/uhdznataly 