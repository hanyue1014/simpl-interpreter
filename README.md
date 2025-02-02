# Simpl
Inspired by [@ThePrimeagen](https://github.com/theprimeagen), specifically [DIC](https://github.com/ThePrimeagen/ts-rust-zig-deez), I have decided to make my own programming language Simpl (specs [below](#language-specs)) in different languages

## Why?
- To take my knowledge of different programming languages I have learnt into **test**
- I have always wanted to try make a language, and an interpreted one seems to be the easiest way to get into

## How?
> To this date, a combination of both following a book and a playlist may be involved, with following a playlist be the primary
-  (Originally wanted to) Based on (book)
    - [Crafting Interpreters](https://craftinginterpreters.com)
- Currently Following a Playlist
    - [Create Your Own Programming Language](https://youtube.com/playlist?list=PLCeDGOId_Kkh4boTj5rGeVn1HQWkzVj_h&si=fRViv6DcHGDNGX9_)
    - [Building a Compiler](https://youtube.com/playlist?list=PLRAdsfhKI4OWNOSfS7EUu5GRAVmze1t2y&si=pFXSOIFRQThT5yrp)

## Language Specs
> I modified the syntax introduced by the various sources a bit (making it closer to my preference), removing certain language features (that maybe will be added back in the future) 

### Variable and Data Types
Variables are dynamically typed (don't wanna add too much complexity to the language), however, the language still has a couple of primitives
```
// bool
true, false

// number
1234, 12.34

// string
"yes, a string"

// for null values
nil

// declaration
let aVariable // defaults to nil
```

### Expressions
Expressions are something that gives a value
```
// arithmetic
1 + 1
1 - 1
1 * 1
1 / 1

// prefix arithmetic
-negation

// comparison
less < than
lessThan <= orEqual
greater > than
greaterThan >= orEqual
equals == to
not != equal

// logical operators (and, or short circuits)
true and false
true or false
!true
```

### Statements
Statements are something that don't give a value
```
print("something")
```

### Functions
Functions are first class items, they can be passed around (may add more ways to declare to challenge myself in the future)
```
// declaring a function
fn function() {
    // function body
    return "returning from a function"
}

fn functionThatTakesFunction(func) {
    func()
}

functionThatTakesFunction(function)
```

