Regular Expressions
===================

Regular expressions can be written as ``r"expression"``, where *expression* is a POSIX compatible regular expression.

.. code-block:: mini

   -- Regular expressions
   r"[0-9]+/[0-9]+/[0-9]+"

:mini:`String / Regex`
   Returns a list of substrings of *String* that were seperated by *Regex*.

:mini:`String % Regex`
   Returns *String* if it matches the pattern in *Regex*.

:mini:`String:find(Regex)`
   Returns the first location of *Regex* in *String*.

:mini:`String1:replace(Regex, String2)`
   Returns a copy of *String1* with every occurence of *Regex* replaced by *String2*. Substitutions are currently not supported in *String2* but see below for an alternative.

:mini:`String:replace(Regex, Function)`
   Returns a copy of *String* with every occurence of *Regex* replaced the result of calling *Function* with any groups matched in *Regex*. The first argument to *Function* is the entire substring matched, followed by the first matched group, then the second and so on.