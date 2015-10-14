String Cases
==========================
2015-10-14



Motivation
--------------

This document can serve as a reference for tools that need to distinguish between different string cases.




Different cases
-----------------------


For all cases, only ascii chars are considered.



- camelCase: starts with a lowercase letter (camelCase, simpleXML, localDb2Remote)
- PascalCase: starts with an uppercase letter
- snake_case: all lowercase letters, words separated with underscores
- CONSTANT_CASE: all uppercase letters, words separated with underscores



Examples
-------------

The table below shows how they translate to each other.


case        |   thisIsNotCorrect    |  simpleXML  |  localDb2Remote   |   notFound404
------------| --------------------- | ------------ |  --------------- |  ----------------
camelCase   |   thisIsNotCorrect    |  simpleXML  |  localDb2Remote   |   notFound404
PascalCase   |   ThisIsNotCorrect    |  SimpleXML  |  LocalDb2Remote   |   NotFound404
snake_case  |   this_is_not_correct    |  simple_xml  |  local_db_2_remote   |   not_found_404
CONSTANT_CASE  |   THIS_IS_NOT_CORRECT    |  SIMPLE_XML  |  LOCAL_DB_2_REMOTE   |   NOT_FOUND_404