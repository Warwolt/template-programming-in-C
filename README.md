# Template Programming in C99
Repository with an example of how to use template programming in C, using only
the preprocessor and some clever conventions.

## Introduction
Generic programming using templates is a common technique in C++, where a piece
of code that is applicable to many different kinds of data (such as sorting
algorithms and storage types) can be defined in a single place. This gets us
around the trouble of duplicating code for each new data type that we want to
support, and frees us from having to maintain all these copies.

When working in C, we don't have any native support for templating as we do in
C++, but we might still want to be able to write generic code to some extent.
With the help of the C preprocessor, as we will see, it is actually possible to
express templates within the C language.

The premise of the technique is to create a file that replaces an explicit type
with a macro, that the client of that file then defines to be the concrete type
that the client wants to work with.

This repository showcases an example of a templated stack abstract data type,
with separated declarations and definitions of functions. Since the technique
is based on the preprocessor, it's possible to utilize both stack-based and
heap-based (opaque pointer) data types.

Since the choice has been to implement the stack as an abstract data type, the
showcase in the repository is heap based.

## Example
(Pictures and code that shows code from the client perspective)

## Structure
(Some UML diagrams showing how all pieces fit together in the implementation)

## References:
1. Lavratti, F. (2016). Template meta-programming in C vs opaque pointer
   [online] Embedded.com. Available at:
   https://www.embedded.com/template-meta-programming-in-c-vs-opaque-pointer/
   [Accessed 15 Dec. 2019].

1. Thrasher, P. (2013). Philip Thrasher's Crazy Awesome Ring Buffer Macros! -
   [online] Github.com. Available at:
   https://github.com/pthrasher/c-generic-ring-buffer/blob/master/ringbuffer.h
   [Accessed 15 Dec. 2019].
