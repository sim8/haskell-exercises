## Lists

Basic list:

```haskell
myList = [1,2,3]
myCharList = ['a', 'b', 'c'] -- strings are syntactic sugar for this
```

Concatenate lists:

```haskell
[1,2] ++ [3,4]
"hello" ++ " " + "world"
"cool" ++ ['!']
-- This is slow if arg 0 is long. Instead:
'a':['b','c'] -- cons operator
```

- `[1,2,3]` is sugar for `1:2:3:[]`
- Everything must be same type
- Can contain lists, but these must be of same type

Extract by index:

```haskell
[1,2,3] : 1 -- 2
"Very nice" : 0 -- 'V'
"Oh no" : 12 -- big fat error
```

Comparison:

```haskell
[1,2,3] > [0,1] -- True
[1,99] > [1,2,3] -- True
"ab" < "v" -- True
```

functions:

```haskell
head [1,2,3] -- 1
last [1,2,3] -- 3
init [1,2,3] -- [1,2]
tail [1,2,3] -- [2,3]
-- All of these break on empty lists
```

Honorable mentions: `length`, `null` (isEmpty), `reverse`
