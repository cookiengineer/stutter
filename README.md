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
let ratio be a Number and set it to 0.37
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


if variable is greater than 2 do

	if variable is greater than 2.5 do
		call log on console with this is an example
	else if variable is lower than 2.5 do
		call alert on console with this is another example
	else
		call log on console with foo bar
	end of condition

end of condition


let examples be a Number Array
set examples to 1, 3, 7 and 9

set index 0 on examples to 4
push 3 to examples


comment whatever is the string representation of examples
let whatever be a String
join examples to whatever

comment copy is the string copy of examples
let copy be a String Array
split whatever to copy


for each examples as key and value do
	let temp be value
	add 5 to value
	divide value by 1.76
	call log on console with temp
end of loop
```


## Implementation Goals

TBD

