
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

In a regex for matching an email, anchors are used to specify the beginning and end of an input string. The caret ( ^ ) anchor is used to indicate the beginning of the string. The dollar sign ( $ ) anchor is used to indicate the end of the string. These are both used to ensure that the regex matches only the email address and not any other text that may appear before or after it. Therefore, the regex will only match to the email and nothing else.  



## Quantifiers



## Grouping Constrcts




## Bracket Expressions



## Charcter Classes



## Flags



## Charcter Escapes
