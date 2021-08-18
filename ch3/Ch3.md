### Use **const** whenever possible

1. to better communicate both to compliers and to other programmers whether a value should remain invariant or not

2. For built-in types and arrays, the lacation of the const qualifier is not important

3. For references,

   >only const reference could refer to a const varaible
   >
   >const referece cannot modify the value of the variable

4. For pointers,

   > If the const is ahead of \*, the pointer points to a constant value, and the pointer cannot modify the value of the varaible; 
   >
   > If the const is behind the \*, the pointer itself is const, which means the address cannot be modified.
   >
   > iterators v.s. const_iterators from STL:
   >
   > > std::vector<double>::iterator  (double \* )
   > >
   > > std::vector<double>::const_iterator (const double \*)



4. For class member function, 

   >- const qualifier helps reduced code duplication when the implementation for const function and non-const function are the same
   >
   >- const qualifier helps interface user whether this api could modify the object or not
   >- const qualifier also makes it possible to work with const objects

5. For error-tracking (superior to preprocessor as indicated in ch2)