# Regex

In this week's challenge we'll be taking a deep look at regex, regular expression, and see exatly what it is that they do. Regular expressions have a large amount of components so they can be very intimidating, however when you look at those components one at a time and try to understand those smaller parts, it will help you long term with having a full understanding of them.

## Summary

Regex is a sequence of characters that create search patterns. They help with matching, locating, and managing texts. Here's a line displaying what regex looks like exactly:

`(\d+(\.\d+)?) (\w+)/`

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

# Regex Components

## Anchors

Anchors are an essential tool for creating more precise regular expressions that match specific patterns within a string. 

The two most common anchors are the caret (^) and the dollar sign . The caret is used to match the beginning of a string or line, while the dollar sign is used to match the end of a string or line. For example, the regular expression "^hello" matches any string that starts with "hello", while the regular expression "world$" matches any string that ends with "world".

1. "^hello" - This matches any string that starts with "hello".
2. "world$" - This matches any string that ends with "world".
3. "\bcat\b" - This matches the word "cat" when it appears as a whole word, and not as part of another word.
4. "\Bdog\B" - This matches the word "dog" only when it appears within another word, and not as a standalone word.
5. "^$" - This matches an empty string.

## Quantifiers

Quantifiers are a powerful tool in regular expressions, allowing you to match patterns that occur multiple times in a string without having to write out each occurrence explicitly.

For example, the regular expression "ab*c" matches strings that start with an "a", followed by zero or more "b"s, and ends with a "c". The regular expression "a{3}" matches strings that have exactly three consecutive "a"s.

1. The asterisk (*) - This matches zero or more occurrences of the preceding character or group of characters.
2. The plus sign (+) - This matches one or more occurrences of the preceding character or group of characters.
3. The question mark (?) - This matches zero or one occurrence of the preceding character or group of characters.
4. The curly braces ({}) - This allows you to specify an exact number of occurrences of the preceding character or group of characters.
5. The curly braces with two values ({min,max}) - This allows you to specify a range of occurrences of the preceding character or group of characters.

## Grouping Constructs

Grouping constructs are a powerful tool in regular expressions, allowing you to create complex patterns and extract specific portions of text from a string.

The regular expression "(ab)*" matches strings that contain zero or more occurrences of the string "ab". The parentheses create a capturing group that allows you to apply the asterisk quantifier to the entire group.

1. Capturing group - This type of group captures the matched text and stores it in a numbered group that can be referenced later in the regular expression or in the replacement string.
2. Non-capturing group - This type of group is similar to a capturing group, but does not capture the matched text. It is often used when you want to group expressions for applying a quantifier, but do not need to store the matched text.
3. Named group - This type of group is similar to a capturing group, but allows you to assign a name to the group for easier reference later in the regular expression or in the replacement string.

## Bracket Expressions

Bracket expressions are enclosed in square brackets and can include a range of characters, as well as metacharacters and escape sequences. Some common metacharacters used in bracket expressions include the caret (^), which is used to negate the character class, and the hyphen (-), which is used to specify a range of characters.

1. "[aeiou]" - This matches any single lowercase vowel.
2. "[a-z]" - This matches any single lowercase letter.
3. "[A-Z0-9]" - This matches any single uppercase letter or digit.
4. "[^aeiou]" - This matches any single character that is not a lowercase vowel.
5. "[\d]" - This matches any single digit character.
6. "[\s]" - This matches any whitespace character (space, tab, newline, etc.).
7. "[\w]" - This matches any word character (letter, digit, or underscore).
8. "[^\w]" - This matches any non-word character.

## Character Classes

In regular expressions, a character class is a shorthand way of matching a specific set of characters. They allow you to define a group of characters that can be matched without having to specify each character individually.

There are several built-in character classes in regular expressions, including:

1. \d - Matches any digit character (0-9).
2. \w - Matches any word character (letter, digit, or underscore).
3. \s - Matches any whitespace character (space, tab, newline, etc.).
4. \D - Matches any non-digit character.
5. \W - Matches any non-word character.
6. \S - Matches any non-whitespace character.

## The OR Operator

The OR operator, denoted by the vertical bar symbol (|), allows you to match one pattern or another. It is used to create a logical "OR" between two or more expressions.

1. "cat|dog" - This matches either "cat" or "dog".
2. "hello|hi|hey" - This matches either "hello", "hi", or "hey".
3. "colou?r" - This matches either "color" or "colour", with the "u" being optional due to the use of the question mark quantifier.
4. "https?://" - This matches either "http://" or "https://", with the "s" being optional due to the use of the question mark quantifier.
5. "jane(|t|s)" - This matches "jane", "janet", or "janes", with the OR operator used to match the optional "t" or "s" at the end of the string.

## Flags

Flags can be set using the syntax "/pattern/flags" in JavaScript and other programming languages that support regular expressions. For example, the regular expression "/hello/i" matches the string "hello" case-insensitively.

1. i - The case-insensitive flag. This makes the regular expression match characters regardless of case.
2. g - The global flag. This causes the regular expression to match all occurrences of the pattern, rather than just the first occurrence.
3. m - The multiline flag. This causes the regular expression to treat the input string as a multiline string, with the ^ and $ anchors matching the beginning and end of each line, rather than just the beginning and end of the entire string.
4. s - The dotall flag. This causes the dot (.) metacharacter to match any character, including newline characters.
5. u - The Unicode flag. This causes the regular expression engine to use Unicode matching rules for characters.

## Character Escapes

A character escape is a way to represent a special character or sequence of characters as a literal string. It allows you to match characters that would otherwise be interpreted as metacharacters or special characters by the regular expression engine.

1. \d - Matches any digit character (0-9).
2. \w - Matches any word character (letter, digit, or underscore).
3. \s - Matches any whitespace character (space, tab, newline, etc.).
4. \D - Matches any non-digit character.
5. \W - Matches any non-word character.
6. \S - Matches any non-whitespace character.
7. \t - Matches a tab character.
8. \n - Matches a newline character.


# Author

Checkout this author's work at https://github.com/alexbrenes999 !
