# Protocols

A protocol defines a set of methods, properties, and other requirements that suit a particular task or piece of functionality. with protocol we define a base.

The protocol can then be followed by a class, structure, or enumeration to provide an actual implementation of those requirements.

Any type that satisfies the requirements of a protocol is said to conform to that protocol.

# Protocol Syntax

We define a protocol like this

```swift
protocol SomeProtocol {
    // protocol definition goes here
}
```

Custom types indicate that they adopt a particular protocol by placing the protocol’s name after the type’s name, separated by a colon, as part of their definition

```swift
struct SomeStructure: FirstProtocol {
    // structure definition goes here
}
```

Multiple protocols can be listed, and are separated by commas:

```swift
struct SomeStructure: FirstProtocol, AnotherProtocol {
    // structure definition goes here
}
```

If a class has a superclass, list the superclass name before any protocols it adopts, followed by a comma:

```swift
class SomeClass: SomeSuperclass, FirstProtocol, AnotherProtocol {
    // class definition goes here
}
```
