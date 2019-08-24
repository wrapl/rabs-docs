Numbers
=======

Numbers in *Minilang* are either integers (whole numbers) or reals (decimals / floating point numbers).

Integers can be written in standard decimal notation. Reals can be written in standard decimal notation, with either ``e`` or ``E`` to denote an exponent in scientific notation. If a number contains either a decimal point ``.`` or an exponent, then it will be read as a real number, otherwise it will be read as an integer.

They support the standard arithmetic operations, comparison operations and conversion to or from strings.

.. code-block:: mini

   -- Integers
   10
   127
   -1
   
   --Reals
   1.234
   10.
   0.78e-12

.. code-block:: mini

   -- Arithmetic
   1 + 1 -- 2
   2 - 1.5 -- 0.5
   2 * 3 -- 6
   4 / 2 -- 2
   3 / 2 -- 1.5
   3 // 2 -- 1
   
   -- Comparison
   1 < 2 -- 2
   1 <= 2 -- 2
   1 = 1.0 -- 1.0
   1 > 1 -- nil
   1 >= 1 -- 1
   1 != 1 -- nil