# Regex:
## Basic topics:
^The        matches any string that starts with The -> Try it!
end$        matches a string that ends with end
^The end$   exact string match (starts and ends with The end)
roar        matches any string that has the text roar in it

## Quantifiers — * + ? and {}
abc*        matches a string that has ab followed by zero or more c -> Try it!
abc+        matches a string that has ab followed by one or more c
abc?        matches a string that has ab followed by zero or one c
abc{2}      matches a string that has ab followed by 2 c
abc{2,}     matches a string that has ab followed by 2 or more c
abc{2,5}    matches a string that has ab followed by 2 up to 5 c
a(bc)*      matches a string that has a followed by zero or more copies of the sequence bc
a(bc){2,5}  matches a string that has a followed by 2 up to 5 copies of the sequence bc
## OR operator — | or []
a(b|c)     matches a string that has a followed by b or c (and captures b or c) -> Try it!
a[bc]      same as previous, but without capturing b or c
## Character classes — \d \w \s and .
\d         matches a single character that is a digit -> Try it!
\w         matches a word character (alphanumeric character plus underscore) -> Try it!
\s         matches a whitespace character (includes tabs and line breaks)
.          matches any character -> Try it!
*Use the . operator carefully since often class or negated character class (which we’ll cover next) are faster and more precise.*

# summary:
1. data validation (for example check if a time string i well-formed)
2. data scraping (especially web scraping, find all pages that contain a certain set of words eventually in a specific order)
3. data wrangling (transform data from “raw” to another format)
4. string parsing (for example catch all URL GET parameters, capture text inside a set of parenthesis)
5. string replacement (for example, even during a code session using a common IDE to translate a Java or C# class in the respective JSON object — replace “;” with “,” make it lowercase, avoid type declaration, etc.)
6. syntax highlightning, file renaming, packet sniffing and many other applications involving strings (where data need not be textual)