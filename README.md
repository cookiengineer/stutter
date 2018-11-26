# Stutter Programming Language

Programming for Humans, not Machines.

(This document currently is a Draft, as the Stutter Language is in its very early stages)


## Design Goals

The design goals of the Stutter Programming Language focus on the underlying idea that Stutter Code
is a speakable language that contains no special syntax characters that are unpronounciable.

Stutter also follows the idea of Composite Pattern, and enforces the usage of simple to pronounciate
verbs as methods on data types and composites. All data types are as simple as possible, meaning
something like "uint8" or "char array" will never land in the language; as they are data types that
machines understand, and humans do not.


**Initial Design Goals**:

- No syntax clutter and no special characters.
- Implicit block scope everywhere.
- Verbs reflect intention and each sentence starts with a verb.
- All methods on all data types (and composites) must be verbs.
- There are no keywords or operators.
- Each sentence ends with a new line separator (`\n`).
- Each sentence may start with a `verb`
- Each sentence follows specific grammar rules.
- Only single line comments are allowed, and the verb `comment` implies a `#` at the beginning of a sentence.
- Only verbs, adverbs and (optionally) adjectives and conjunctions are allowed between references.

A simple example with valid stutter code:

```stutter
let ratio be a Number with the value 0.37
let variable be a Number
set variable to 5

comment add is a method on the Number data type
add 12.0 to variable

comment all methods accept multiple parameters via the and conjunction
multiply variable with ratio and 1.5

comment results of methods can be redirected with the to preposition
print variable to standard output

comment generic calls can be done with the call verb
call log on console with variable and ratio
```


## Implementation Goals

TBD

