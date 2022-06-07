# japanese-goblinn's Swift Style Guide

- Using [swiftlint](https://github.com/realm/SwiftLint) is the best way to maintain consistent code style and share it with others.

## General

- Use tab width equal to `2` spaces instead of default `4`

## Control Flow

### `if` statement

```swift
// 🛑
if condition { doStuff() }

// ✅
if condition {
  doStuff()
} 

// ✅✅
condition ? doStuff() : () 
```

## Enums

```swift
// If enum is used for namespacing - use plural name
enum Deeplinks {
  struct Universal {}
  struct URLSchema {}
}

// In other cases use singular name
enum State {
  case idle
  case loading
}
```

## Resources

- [Swift.org - API Design Guidelines](https://www.swift.org/documentation/api-design-guidelines/)