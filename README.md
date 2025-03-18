# Lexer-Implementation
<br>
This project is a Java lexer implemented in Python, designed to tokenize Java source code without using regular expressions. Instead, it relies on pure programming logic to analyze the structure of the code and identify tokens such as keywords, identifiers, literals, operators, and symbols.
<br>
<br>

# Features
<br>
Tokenizes Java source code without using regex.
<br>
Supports Java keywords, identifiers, operators, literals, and symbols.
<br>
Implements a rule-based approach for token extraction.
<br>
Handles multi-line and single-line comments.
<br>
Efficient character-by-character parsing mechanism.
<br>

# Example
<br>
Input (Java Source Code) <br>
import javax..@@*;<br>
<br>
++c++ == 20.23.34;<br>
<br>
//comments<br>
/*<br>
x= 20;<br>
*/<br>
<br>
{{}}<<??: hello<br>
"w0.4ssdglkwe";<br>
'c'<br>
#int __3$ = 20;<br>
  
# Output (Tokenized Representation) <br>
-----------Tokens------------<br>
[Line:2] [import]: Reserved Word<br>
[Line:2] [javax]: Identifier<br>
[Line:2] [.]: Special Symbol<br>
[Line:2] [.]: Special Symbol<br>
[Line:4] [++]: Special Symbol<br>
[Line:4] [c]: Identifier<br>
[Line:4] [++]: Special Symbol<br>
[Line:4] [==]: Special Symbol<br>
[Line:4] [;]: Special Symbol<br>
[Line:11] [{]: Special Symbol<br>
[Line:11] [{]: Special Symbol<br>
[Line:11] [}]: Special Symbol<br>
[Line:11] [}]: Special Symbol<br>
[Line:11] [<]: Special Symbol<br>
[Line:11] [<]: Special Symbol<br>
[Line:11] [hello]: Identifier<br>
[Line:12] [w0.4ssdglkwe]: Single Line String<br>
[Line:12] [;]: Special Symbol<br>
[Line:13] ['c']: Charecter<br>
[Line:14] [=]: Special Symbol<br>
[Line:14] [20]: INTEGER<br>
[Line:14] [;]: Special Symbol<br>
-----------Errors-------------<br>
Line [2]:[@@*;] Invalid<br>
Line [4]:[20.23.34] Invalid<br>
Line [11]:[??:] Invalid<br>
Line [14]:[#int] Invalid<br>
Line [14]:[__3$] Invalid<br>
