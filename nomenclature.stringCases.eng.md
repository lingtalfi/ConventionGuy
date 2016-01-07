String Cases
==========================
2015-10-14



Motivation
--------------

This document can serve as a reference for tools that need to distinguish between different string cases.




Different cases
-----------------------


A word contains only the [a-Z0-9_] chars.
A wordChar is a char in the [a-Z0-9_] range.




- camelCase: everything to lower case, then change the first letter of each word but the first to uppercase, then remove gaps between words  
- flexibleCamelCase: change the first letter of each word but the first to uppercase, then remove gaps between words  
- PascalCase: everything to lower case, then change the first letter of each word to uppercase, then remove gaps between words
- FlexiblePascalCase: change the first letter of each word to uppercase, then remove gaps between words 
- snake_case: everything to lower case, then replace gaps between words with one underscore (_). Characters other than undercores, flat letters (non accentuated) and numbers are stripped out
- dash-case: replace consecutive blanks with one dash
- hotDog-case: keep original case, and replace any non **wordChars** with a dash. No dash can precede another dash
- dog-case: everything to lower case, and replace any non **wordChars** with a dash. No dash can precede another dash
- CONSTANT_CASE: everything to upper case, then replace gaps between words with one underscore (_)


### Snake case

A string with everything to lower case.
Accepted characters are underscores, the 26 letters of the alphabet lower case, and the digits.
Characters outside of this range are stripped out.
Consecutive underscores are replaced with one underscore.


### Dog case

A string with everything to lower case.
Accepted characters are underscores, the 26 letters of the alphabet lower case, the digits, and the dash.
Characters outside of this range are stripped out.
Consecutive dashes are replaced with one dash.





Examples
-------------

The table below shows how they translate to each other.


case        |   this is not correct |  simple XML  |  local db 2 remote   |    XML element
------------| --------------------- | -------------------  | ------------ |  ---------------  
camelCase   |   thisIsNotCorrect   | simpleXml  |  localDb2Remote   |     xmlElement
flexibleCamelCase |  thisIsNotCorrect   |  simpleXML  |  localDb2Remote  | XMLElement
PascalCase   |   ThisIsNotCorrect   | SimpleXml  |  LocalDb2Remote   |   XmlElement 
FlexiblePascalCase   | ThisIsNotCorrect  |  SimpleXML  |  LocalDb2Remote  | XMLElement 
snake_case  |   this_is_not_correct  |  simple_xml  |  local_db_2_remote  | xml_element
dog-case  |   this-is-not-correct  |  simple-xml  |  local-db-2-remote  | xml-element
CONSTANT_CASE  |  THIS_IS_NOT_CORRECT  |  SIMPLE_XML  |  LOCAL_DB_2_REMOTE  | XML_ELEMENT 





History Log
------------------
    
- 2.0 -- 2015-11-07

    - reforged cases definitions
    
    
- 1.0 -- 2015-10-14

    - initial commit
    
    