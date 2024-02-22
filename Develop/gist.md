# Matching an Email Using REGEX

By Phil Sloan


As you fall into the rabbit-hole of regex, you will be entering a world of precision and pattern matching. The art of identifying email addresses through regular expressions requires attention to detail and a keen eye for patterns. With the right approach(and teacher), you can efficiently sift through strings of text, uncovering the email addresses hidden within. So, with this newfound knowledge, GO! Set forth on this venture of discovery and ultimatley TRIUMPH! Take head and be ready to conquer the challenges that lie ahead. Good luck.......

## Summary

Here it is ..... 

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

This is your example of matching the proper emails while you traverse this ancient and fragile document. Use it and read through VERRRRY carefully. One mis-placed keystroke could mean...... devestation......

Or you won't find the write email addy's ya silly goose! I'm trying to make this fun dangit, this class is hard....

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Just Checkin' in](#just-checkin'-in)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors

^   $   ^   $   ^   $

The regular expression employed for email matching incorporates specific anchors: '^' denotes the start of the string, while '$' signifies its conclusion. It's crucial to note that the multiline flag '(m)' isn't activated, meaning the regex interpretation concludes upon encountering '$'. In essence, these anchors delineate the exact boundaries within which the regex engine operates, ensuring precise email identification within the text.

### Quantifiers

A quantifier defines the quantity of occurrences required for the preceding element, which could be a character, a group, or a character class, to constitute a match within the input string. In simpler terms, it dictates the number of times a specific element must appear for the regex pattern to successfully match against the text being evaluated.

In an email address, various components like the local part (before the '@' symbol) and the domain part (after the '@' symbol) have different requirements regarding the number of characters they can contain.

### OR Operator

OR operators can be useful when defining patterns that accommodate variations in email formats. Email addresses can have different structures, and regex patterns must be flexible enough to handle these variations.

For example, email addresses can have different domain types, such as ".com", ".org", ".net", etc. Using an OR operator, you can create a regex pattern that matches any of these domain types.

### Character Classes

There are several Character Classes you need to understand when trying to match emails using REGEX. We'll start with Bracket Expression.

Bracket expressions, denoted by square brackets [], are used to specify a set of characters that the regex engine should match. They allow you to define custom character classes that can match any character within the set.

In the context of matching emails using regex, bracket expressions are commonly used to define character classes for the local part (before the '@' symbol) and the domain part (after the '@' symbol) of the email address.

Those character classes include..

1. Alphanumeric Characters: [A-Za-z0-9]
2. Special Characters: ['.','%', '+''.', '_', '%', '+', and '-']
3. Domain Characters: [A-Za-z0-9.-]
4. Top-level Domain Characters: [A-Za-z] - TLDs are usually composed of letters only, such as ".com", ".org", ".net", etc.


### Grouping and Capturing

By using grouping and capturing effectively in your regex pattern, you can not only match emails but also extract and manipulate specific components of the email addresses as needed.

Grouping, denoted by parentheses (), allows you to define subpatterns within your regex. This is useful for specifying sections of the pattern that should be treated as a single unit. 

Capturing, also facilitated by grouping, is the process of extracting the text matched by a specific group in the regex pattern. When a regex match occurs, each group captures the portion of the matched text that corresponds to its subpattern. This allows you to retrieve and work with specific parts of the matched text.


## Just Checkin' in

Are you still with me? If you're confused imagine how I felt typin' and researchin' the dang topic. But fear not weary traveller. Let's go over something we all ready know!

### Bracket Expressions

Bracket expressions, also known as character classes, are a fundamental component of regular expressions used for pattern matching. They allow you to specify a set of characters that the regex engine should match. For example, [abc] would match any single character that is either 'a', 'b', or 'c'. These expressions are enclosed within square brackets [], and they provide a convenient way to define custom sets of characters that fulfill specific matching criteria. Bracket expressions offer flexibility in defining patterns by allowing you to match a single character from a predefined set of options.

See? it's getting easier!!!

### Greedy and Lazy Match

Greedy and lazy matching can be important considerations depending on the structure of the email addresses you are trying to match. Greedy matching may lead to overmatching if not used carefully, while lazy matching can help ensure more precise matches by stopping at the earliest opportunity.

Greedy matching, which is the default behavior of most regex engines, attempts to match as much text as possible while still allowing the overall pattern to match. This means that the quantifier will match as many characters as it can, potentially resulting in a longer match than desired.

Lazy matching, on the other hand, attempts to match as little text as possible while still allowing the overall pattern to match. This is achieved by adding a question mark ? after the quantifier. 

Rember what Quantifiers are? I didn't I had to look back and re-read it like 6 times....

### Boundaries

By using boundaries in your regex pattern, you can ensure that the pattern matches email addresses within the desired context, such as when they appear at the beginning or end of a line.

The caret symbol (^) asserts the start of the line or string. When placed at the beginning of a regex pattern, it ensures that the pattern only matches if it starts at the beginning of the input text.

That seems familiar.....

The dollar symbol ($) asserts the end of the line or string. When placed at the end of a regex pattern, it ensures that the pattern only matches if it ends at the end of the input text. 

### Back-references

Back-references are helpful for ensuring consistency and validation within complex regex patterns, including those used for matching emails.

 If you want to ensure that the domain part matches exactly the same characters as the local part, you can use a back-reference. They will ensure that the domain part matches exactly the same characters as the local part, providing additional validation for the email address format.

### Look-ahead and Look-behind

These are assertions that provide a powerful way to add additional conditions or constraints to regex patterns when matching emails, allowing for more precise and flexible matching based on specific requirements or criteria.

Look-ahead assertions, denoted by (?=...), specify a condition that must be met after the current position in the string for the match to succeed.

Look-behind assertions, denoted by (?<=...), specify a condition that must be met before the current position in the string for the match to succeed. 

## Author

I, the author of this captivating dive of tech info, am Phil "The Chill" Sloan. Some say I come across as "cold". While I like to think I come across as... "Cooool".
My coding is much better than my dad jokes. Reach out to me if you're intrested in knowing what I can accomplish when I'm apart of a colaberative team!

email- pjs.tgj@fatmail.com
github- https://github.com/philsloan/
Phone Number- yah right, I don't need any more spam calls or "The Chill" might turn into "The KILL"...........