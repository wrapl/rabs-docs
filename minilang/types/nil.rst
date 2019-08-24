Nil
===

The special built in value :mini:`nil` denotes the absence of any other value. Every variable has the value :mini:`nil` before they are assigned any other value. Likewise, function parameters default to :mini:`nil` if a function is called with too few arguments.

.. note::

   *Minilang* has no boolean values, such as ``true`` or ``false``. Instead, conditional and looping statements treat :mini:`nil` as false and *any* other value as true.  

.. code-block:: mini

   -- Nil
   nil
   
   if nil then
      print("This will not be seen!")
   end
   
   if 0 then
      print("This will be seen!")
   end

.. _comparisons:

In *Minilang*, comparison operators such as :mini:`=`, :mini:`>=`, etc, all return the second argument if the comparison is true, and :mini:`nil` if it is not.

.. code-block:: mini

   1 < 2 -- returns 2
   1 > 2 -- returns nil 