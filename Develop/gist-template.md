# Finding a URL with regex

\b(https?:\/\/)?(www.)?([\da-z\.-]+)\.([a-z\.]{2,6})\b

I will be explaining the following regex

## Summary/Explanation

This piece of regex find a URL that may or may not have 'https://' or 'http://', and may or may not have 'www.'. Followed by the name of the site that with digits, letters a-z, a period, and a dash. Proceeded by a period. While lastly being followed by letters a-z and a period with a minimum length of 2 and maximum length of 6.

## Table of Contents

- [Literals](#literals)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping)
- [Bracket Expressions](#bracket-expressions)
- [Boundaries](#boundaries)
- [Meta Characters](#meta-characters)
- [Author](#author)

## Regex Components

The following components were used in this expression:

\b
()
\/
?
[]
+
\.
{min, max}

### Literals

'\.': The back slash allows you to escape the meta meaning of '.' and lets you use the literal meaning of '.'
'-': This literally means '-'
'\/': The back slash allows you to escape the meta meaning of '/' and let you use the literal meaning '/'

### Quantifiers

'+': The plus quantifier stands for one or more.
'?': The question mark quantifier stands for optional
'{}': can be used as {n} to have a set amount of what preceeds it or {min, max} to set boundaries on what preceeds it.

### Character Classes

'[]': Character Classes are used to set boundaries within things like characters [a-z], [A-Z], [0-9]. Perhaps you only want [a-f] or [0-5].

### Grouping

'()': The entire text you're looking at is known as Group 0 and then every part of the expression you encase in () is incremented by 1 and goes from left to right of the regular expression

### Bracket Expressions

'{}': Bracket expressions are used to set the paramters of what is preceding it like we seen in the quantifier section for '{}'.

### Boundaries

'\b': Word Boundaries are used to look if there are white spaces before or after.

### Meta Characters

'\d': This is the same as using a Character class [0-9]
'\w': This is the same as using [A-Za-z0-9].

## Author

The purpose of this project is to simultaneously help someone who's trying to learn regex while also deepening my understanding of it as well. Checkout my github!
https://github.com/JaviD17
