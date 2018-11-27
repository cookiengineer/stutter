
# Sentence

A sentence in Stutter always has the same specific structure.

A Subject refers to a declared Variable or Reference in the
current Scope. The Object refers to a Value or a declared Variable
or Reference.

```
verb <Subject> (preposition) <Object>
if <Condition>
```

Example:

```stutter
let value be a Number and set it to 1
let result be a Number and set it to 2

multiply whatever with 2 to result
```


## Primitive Verbs

Primitive Verbs are reserved and cannot be used as Verbs for
specific Types. These Verbs are included in the language
and cannot be overwritten and neither be modified.

These Verbs fall into the Primitive Verbs category:

- `break`
- `call`
- `comment`
- `end`
- `let`
- `set`


### let

The `let` Verb allows the declaration of a variable for the
current Scope, and allows optionally an additional assignment
chained with the `and` Preposition.

The grammatical structure of its usage is:

```stutter
let <Identifier>
let <Identifier> be a <Type>
let <Identifier> be a <Type> and set it to <Value>
```

### set

The `set` Verb allows the assignment of a Type-specific Value
to an already declared Variable in the current Scope.

The grammatical structure of its usage is:

```stutter
set <Reference> to <Value>
```


## Operators



## Conditions

Conditions always follow the same structure and allow the
implementation of logic in the program code based on operators.


## Loops

- for each variable as key and value do
- while variable lower than x do

```stutter

```

