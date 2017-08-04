# Regular Expression (RegEx) Resources

> "Some people, when confronted with a problem, think 
“I know, I'll use regular expressions.”   Now they have two problems." - Jamie Zawinski

Regular Expressions are a powerful meta-syntax for describing search patterns. They can be difficult to understand when you first get started, but once you get the basics, you will find myriad uses for them in your day-to-day work. Everything from your command line (grep, sed, awk) to your editor (Atom, VS Code, Sublime, etc.) to your language-of-choice (Ruby, JavaScript, PHP, Python, Java, Perl, etc.) supports RegEx. You'll find that your programs and your workflow are enhanced greatly by an understanding of this powerful search syntax. 


## Regular Expression Tools
* **[RegEx101.com](https://regex101.com/)** - Handy tool for testing your RegEx in real-time. Great resource for _explaining_ how your RegEx works!
* **[RegExr](http://regexr.com/)** - An online tool to build, test and learn RegEx
* **[Rubular](http://www.rubular.com/)** - A Ruby regular expression editor

## Simple Examples
* `<[^>]*>` - Finds all HTML tags in a string
* `<([^>\s]*)([^>]*)>(.*)<\/\1>` - Finds an instance of an HTML tag and returns 3 backreferences for the tag, attributes and innerText.
* `'(800) 555-1212'.replace(/[^0-9]/g,'');` - Returns only the numbers in the phone number (JS Syntax)


## Basic Language Reference
There are many online resources for learning RegEx, as well as a number of good books, such as [Mastering Regular Expressions](http://amzn.to/2ur3fDO), [Regular Expressions Cookbok](http://amzn.to/2u8gtpA) and [Regular Expressions Pocket Reference](http://amzn.to/2wdGRQF), all from O'Reilly. Here is a simple syntax reference that covers the basics of the language.

### Brackets
* `[abc]` Find any character between the brackets
* `[^abc]` Find any character NOT between the brackets
* `[0-9]` Find any number between the brackets
* `[^0-9]` Find any number NOT between the brackets
* `(a|b)` Find any of the characters (a or b)

### Metacharacters
* `.`	Find a single character, except newline or line terminator
* `\w`	Find a word character
* `\W`	Find a non-word character
* `\d`	Find a digit
* `\D`	Find a non-digit character
* `\s`	Find a whitespace character
* `\S`	Find a non-whitespace character
* `\b`	Find a match at the beginning/end of a word
* `\B`	Find a match not at the beginning/end of a word
* `\0`	Find a NUL character
* `\n`	Find a new line character
* `\f`	Find a form feed character
* `\r`	Find a carriage return character
* `\t`	Find a tab character
* `\v`	Find a vertical tab character

### Quantifiers
* `n+`	Matches any string that contains at least one n
* `n*`	Matches any string that contains zero or more occurrences of n
* `n?`	Matches any string that contains zero or one occurrences of n
* `n{X}`	Matches any string that contains a sequence of X n's
* `n{X,Y}`	Matches any string that contains a sequence of X to Y n's
* `n{X,}`	Matches any string that contains a sequence of at least X n's
* `n$`	Matches any string with n at the end of it
* `^n`	Matches any string with n at the beginning of it
* `?=n`	Matches any string that is followed by a specific string n
* `?!n`	Matches any string that is not followed by a specific string n

