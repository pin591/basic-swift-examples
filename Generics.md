# Generics

## What exactly generics are?

One of the most powerful característics of the Swift language.
Generic programming is a way to write functions and data types while making minimal assumptions about the type of data being used.
It allows you to write a function once and use it on different types.
Allowing for elegant abstractions that produce cleaner code with fewer bugs. 

You’ll find generics in use throughout Swift, which makes understanding them essential to a complete mastery of the language.
A hight average of the standard swift libraries are write with generic code (Array, Dictionary, Optional, Results...) You can have an array or an optional for example of any data type you want, even those types you create yoursel. In other words, the Optional data type is generic over the type of value it might contain.

the Optional data type is generic over the type of value it might contain.

## Why they are useful?

## How to write generic functions

This is a simple example that demonstrates Swift’s type safety. You can call this function with two integers, but not any other type

```swift

func addInts(x: Int, y: Int) -> Int {
  return x + y
}

let intSum = addInts(x: 1, y: 2)

```

```swift

func addDoubles(x: Double, y: Double) -> Double {
  return x + y
}
```
let doubleSum = addDoubles(x: 1.0, y: 2.0)


The function signatures of addInts and addDoubles are different, but the function bodies are identical. Do you have two functions, but the code inside them is repeated. Generics can be used to reduce these two functions to one and remove the redundant code.
Generics can be used to reduce these two functions to one and remove the redundant code.

## How to write generic data structures

## How to use type constraints.

## How to extend generic types
