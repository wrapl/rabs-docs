Strings
=======

Strings can be written in two ways:

Regular strings are written between double quotes ``"``, and contain regular characters. Special characters such as line breaks, tabs or ANSI escape sequences can be written using an escape sequence ``\n``, ``\t``, etc.

Complex strings are written between single quotes ``'`` and can contain the same characters and escape sequences as regular strings. In addition, they can contain embedded expressions between braces ``{`` and ``}``. At runtime, the expressions in braces are evaluated and converted to strings. To include a left brace ``{`` in a complex string, escape it  ``\{``.

.. code-block:: mini

   -- Regular strings
   "Hello world!"
   "This has a new line\n", "\t"
   
   -- Complex strings
   'The value of x is \'{x}\''
   'L:length = {L:length}\n'
  
:mini:`String:length`
   Returns the length of *String*.

:mini:`String:trim`
   Returns a copy of *String* with whitespace removed from either end.

:mini:`String[I]`
   returns the *I*-th byte of *String* as a a string of length 1. Negative indices are taken from the end of the string.

:mini:`String[I, j]`
   Returns the substring of *String* starting at *I* and ending just before *J*. Negative indices are taken from the end of the string.

:mini:`String1 + String2`
   Returns the concatenation of *String1* and *String2*.

:mini:`String1 / String2`
   Returns a list of substrings of *String1* that were seperated by *String2*.

:mini:`String1 % String2`
   Returns *String1* if it matches the pattern in *String2* (as a regular expression).

:mini:`String1:find(String2)`
   Returns the first location of *String2* in *String1*.

:mini:`String1:replace(String2, String3)`
   Returns a copy of *String1* with every occurence of *String2* replaced by *String3*.
