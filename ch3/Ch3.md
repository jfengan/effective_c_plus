### Use **const** whenever possible

1. to better communicate both to compliers and to other programmers whether a value should remain invariant or not

2. For built-in types and arrays, the lacation of the const qualifier is not important

3. For pointers,

> If the const is ahead of \*, the pointer points to a constant value, and the pointer cannot amend the value of the varaible; 

> If the const is behind the \*, the pointer itself is const, which means the address cannot be amended.