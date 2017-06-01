Jupyter notebooks for "Fluent Python", by Luciano Ramalho
=========================================================

![cover](http://akamaicovers.oreilly.com/images/0636920032519/cat.gif "Cover")

## Chapter One - The Python Data Model

The book starts with a chapter on the Python data object, highlighting the advantages of using special methods (aka dunder methods), as they give access to core language features — like iteration and slicing from the standard library. A small class is created, that implements some special methods. From there, slice and choice are used, without having programmed them. It is clear from the example that one of the biggest advantages of using Python's magic methods is that they provide a simple way to make objects behave like built-in types. That means you can avoid ugly, counter-intuitive, and nonstandard ways of performing basic operators. For example, the __add__ dunder method is implmented to enable the adding of two dictionaries, where the + operand is not supported by the 'dict' type.

## Chapter Two - An Array of Sequences

Chapter 2 dives into the Python sequence types, based on the C primitives. Firstly, the list type is discussed, including list comprehension and generator expressions, for creating lists and Cartesian products. These are compared with for loops, and map and filter functions. Secondly tuples are covered, both as records with no names, and immutable lists. This includes tuple unpacking, named tuples and the associated special attibutes, such as `__make` and `__asdict`. Thirdly, there is the a good section on slicing, nested lists, augmented assignment and sorting. There are a few exercises that cover list searching using `bisect` and large lists in arrays. Fourthly, there is a section on memory views, which allow direct manuipulation of data objects through byte poking. The last section introduces NumPy as a means of handling 2D arrays, and queues as a means of handling fixed length sequences. 

## Chapter Three - Dictionaries and sets

The third chapter focuses on dictionaries and sets, which are widely used and fast data structures. It outlines some real world uses, such as module namespaces, and discusses dict comprehension syntax. There is then a discussion of some of the standard dict types - such as defaultdict and ordered dict, and the available methods, like default key, missing key. There is a section dedicated to the UserDict type, and the relevant built-ins. Mapping proxy is highlighted as a read-only, but dynamic view of a dict. Finally, there is a summary of set theory, and hash tables, which explains why dicts must be immutable, why lookup is so fast, and why there is a memory overhead.

## Chapter Four - Text vs Bytes

The author works through the unicode standard, and the various encodings which implement it. A couple of examples are used to illustrate encoding and decoding a non-ASCII character, and the Python byte sequences are introduced, followed by struct and memory views. A few different encoders are discussed, including files encoding and default system encoding. The chapter goes onto show how mixed characters can be normalised, casefolded and sanitised, and stripped of diacritics. A short function displays the unicode database, including some metadata.

## Chapter Five - First-class functions

This chapter deals with one of the key features of Python - functions being first-class objects. This means they can be created at runtime, assigned to var or element, passed as an argument or returned as a result. The idea of a higher-order function is introduced, being a function that takes another function as an argument. Then anonymous functions are introduced, as well a different types of callable object. Some nice examples of positional and keyword arguments are introduced, as well as introspection using passive attributes like co_varnames & annotations, and more advanced modules such as inspect. There is also a brief introduction to functional programming operators and funtools.

## Chapter Six - Design patterns with first-class functions

A relatively brief chapter, the advantages of functions as first class objects are reinforced through the refactoring of a couple of design patterns, as listed in the famous 'Gang of Four' design pattern book. The Strategy design pattern is particularly clearly discussed, with functions being passed as objects to disassocate them from a particular class.

## Chapter Seven - Function decorators and closures

This chapter covers a lot of ground, and does a really solid job of explaining decorators, closures, nonlocal vars and nested functions. Each term is given a good definition, and then the interplay and interdependencies of the different entities is explained. The chapter closes with some standard library decorators, and then goes on to establish a custom decorator, which is passed arguments, and customised even further. The final examples are quite complex, but should help to clarify a lot of the 'framework magic' used in e.g. Flask and Django.

 