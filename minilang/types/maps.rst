Maps
====

Maps are extendable collections of key-value pairs, which can be indexed by its keys. Maps are created using braces ``{`` and ``}``. Keys can be of any immutable type supporting equality testings (typically numbers and strings), and different types of keys can be mixed in the same map. Each key can only be associated with one value, although values can be any type, including lists, other maps, etc.

:mini:`Map:size`
   Returns the number of key-value pairs in *Map*.

:mini:`Map[Key]`
   Returns an assignable reference to the value associated with *Key* in *Map*. If *Key* is not currently in *Map* then returns :mini:`nil`. Assigning to :mini:`Map[Key]` will overwrite the associated value or insert a new association if *Key* is not already in *Map*.
   
:mini:`Map:insert(Key, Value)`
   If *Key* is present in *Map*, then the association is replaced with *Value*, and the old value associated with *Key* is returned. Otherwise *Key* is inserted into *Map* associated with *Value*, and :mini:`nil` is returned. 

:mini:`Map:delete(Key)`
   If *Key* is in *Map* then it removed from *Map* and the associated value is returned. Otherwise *Map* is unchanged and :mini:`nil` is returned.

:mini:`Map:join(Sep1, Sep2)`
   Returns *Map* converted to a string with *Sep1* between each key and its associated value and *Sep2* between each key-value pair.

:mini:`for Value in Map do ... end`
   Iterates through the values in *Map*. *Value* is an assignable reference, assigning to *Value* replaces the element in *Map*.

:mini:`for Key, Value in Map do ... end`
   Iterates through the keys and associated values in *Map*. *Value* is an assignable reference, assigning to *Value* replaces the element in *Map*.

:mini:`Map1 + Map2`
   Returns a new map containing all of the key-value pairs in *Map1* and *Map2*. If the same key is in both maps, then the associated value is taken from *Map2*.


  