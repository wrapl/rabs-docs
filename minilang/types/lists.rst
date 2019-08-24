Lists
=====

Lists are extendable ordered collections of values, and are created using square brackets, ``[`` and ``]``. A list can contain any value, including other lists, maps, etc.

:mini:`List[I]`
   Returns an assignable reference to the *I*-th element of *List*. If *I* is negative, then the indexing is done from the end *List*, where ``-1`` is the last element. If *I* is outside the bounds of *List*, then :mini:`nil` is returned.
   
:mini:`List[I, J]`
   Returns the sub-list of *List* starting with the *I*-th element up to but excluding the *J*-th element. Negative indices are taken from the end of *List*. If either *I* or *J* it outside the range of *List*, or *I* > *J* then :mini:`nil` is returned.
   
:mini:`List:put(X1, X2, ...)`
   Puts *X1*, *X2*, ... onto the end of *List* and returns *List*.
   
:mini:`List:push(X1, X2, ...)`
   Puts *X1*, *X2*, ... onto the beginning of *List* and returns *List*.
   
:mini:`List:pull`
   Removes and returns the last element of *List*, or :mini:`nil` if *List* is empty.
   
:mini:`List:pop`
   Removes and returns the first element of *List*, or :mini:`nil` if *List* is empty.
   
:mini:`List1 + List2`
   Returns the concatenation of *List1* and *List2*.
   
:mini:`List:length`
   Returns the number of elements in *List*.
   
:mini:`List:string`
   Returns *List* converted to a string.
   
:mini:`List:join(Sep)`
   Returns *List* converted to a string with *Sep* between each element.

:mini:`for Value in List do ... end`
   Iterates through the values in *List*. *Value* is an assignable reference, assigning to *Value* replaces the element in *List*.

:mini:`for Index, Value in List do ... end`
   Iterates through the indices and values in *List*. *Value* is an assignable reference, assigning to *Value* replaces the element in *List*.

:mini:`List1 + List2`
   Returns a new list with the elements of *List1* followed the elements of *List2*.