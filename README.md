# kaboom
This is a part of my coding night exercise...
image rendering

## C++ Learning
##### size_t
```size_t``` alias for an unsigned integer type. Able to represent size of an object in bytes.

##### typedef
```typedef``` a different name through which a type can be identified. Any valid datatype can be aliased so that it can be referred to with a different identifier.

 
```define _USE_MATH_DEFINES``` Used to invoke some custom symbols for mathematical constants.

```#include <algorithm>``` defines a collection of functions especially designed to be used on the ranges of elements.

##### Inline function specifier
keyword ```inline``` Inline function is introduced which is an optimization technique used by the compilers especially to reduce the execution time. The inline functions are a C++ enhancement feature to increase the execution time of a program. Functions can be instructed to compiler to make them inline so that compiler can replace those function definition wherever those are being called. Compiler replaces the definition of inline functions at compile time instead of referring function definition at runtime.\
So does it mean that ```inline``` instructs the compiler to consider the whole function instead of just the function call at the compile time. Yes. Inline means to take the entire function description in the main function while avoiding jumps to the function declaration.

##### Templates
Basically a template is used when a function or a class or a variable happens to be used often with different datatypes in the code.\
For example:
```
template <typename T> inline T lerp(const T &v0, const T &v1, float t) {
    return v0 + (v1 - v0)*std::max(0.f, std::min(1.f, t));
}
```

Here in this piece of code,\
```template``` keyword declares the template.\
```<typename T>``` defines datatype identifier typename with value T.\
```inline``` see above.\
```T lerp``` function datatype and function name.\
```(const T &v0, const T &v1, float t)``` initializes the arguments of the function with datatype T.

##### Hash Functions
A hash function is any function that can be used to map data of arbitrary size to fixed-size values. 

## Some Graphics Concepts

```Perlin Noise```
- [Perlin](https://adrianb.io/2014/08/09/perlinnoise.html) Noise can be used for any sort of wave-like, undulating material or texture.

```lerp function```
- [Lerp](https://lunarlabs.pt/blog/post/the_art_of_lerp) means linear interpolation, and is used to "mix" two values (we'll call them A and B) based on a third value, a percentage, which we will call X for now (depending on the engine and language, you might see it be called T, S or even other letters!). The third value (X) is a float value from 0 to 1, which you can think as a percentage that goes from 0 to 100%. Other way to visualize it, is to imagine a line with value A in the left, and value B in the right. The interpolation value will be used to pick a number in between. That's where the "linear" comes from.\
```lerp(v0, v1, t) = v0 + (v1 - v0)*t```






