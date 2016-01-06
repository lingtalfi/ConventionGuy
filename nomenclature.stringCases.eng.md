String Cases
==========================
2015-10-14



Motivation
--------------

This document can serve as a reference for tools that need to distinguish between different string cases.




Different cases
-----------------------


A word contains only the [a-Z0-9_] chars.




- camelCase: everything to lower case, then change the first letter of each word but the first to uppercase, then remove gaps between words  
- flexibleCamelCase: change the first letter of each word but the first to uppercase, then remove gaps between words  
- PascalCase: everything to lower case, then change the first letter of each word to uppercase, then remove gaps between words
- FlexiblePascalCase: change the first letter of each word to uppercase, then remove gaps between words 
- snake_case: everything to lower case, then replace gaps between words with one underscore (_). Characters other than undercores, letters and numbers are stripped out.
- CONSTANT_CASE: everything to upper case, then replace gaps between words with one underscore (_)






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
CONSTANT_CASE  |  THIS_IS_NOT_CORRECT  |  SIMPLE_XML  |  LOCAL_DB_2_REMOTE  | XML_ELEMENT 





History Log
------------------
    
- 2.0 -- 2015-11-07

    - reforged cases definitions
    
    
- 1.0 -- 2015-10-14

    - initial commit
    
    