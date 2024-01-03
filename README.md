# tsort

An implementation of POSIX tsort.

See https://pubs.opengroup.org/onlinepubs/9699919799/utilities/tsort.html

This implementation performs in roughly linear time using the classic Knuth algorithm Algorithm T, Topological sort, from The Art of Computer Programming Vol 1, sec. 2.2.3.

If a cycle is detected, this program prints a single cycle to assist in resolving the problem, using the solution to Knuth sec. 2.2.3 Exercise 23.
For example, given the input `a b b c c a c d d e`, it prints
```
input contains a loop:
a ->
b ->
c ->
a
```

It is heavily commented to show where the code corresponds with Knuth's description.

Licensed 0BSD, free for any use.
