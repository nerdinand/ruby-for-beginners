# Arrays

*Arrays are like bags that contain things*

While numbers, strings, and symbols all represent simple, primitive things,
arrays are more interesting, and very useful.

Arrays are things that store (or "hold") other things.

You can think of an array as a collection or list of things. Or better yet, as
a bag that you can throw things in: The bag itself is a thing (an object), too.

An array is created by separating values by commas, and enclosing this list
with square brackets, like so:

```ruby
[1, 2, 3]
```

Or:

```ruby
["A string", 1, :some_symbol, 2]
```

This creates an array with 4 elements, i.e. a bag that contains 4 things: a
string, a number, a symbol, and another number.

Note that in Ruby arrays always keep their order (unless you do something
to change the order).

Also note that in Ruby you can store any kind of object in an array. For
example, you can also store arrays in an array: that's a 2-dimensional array,
like a table that has many rows, and each row has many cells ("things").

Arrays can be used in a lot of different, and useful ways, but the most basic
one is to retrieve a certain element by the way of referring to its position:
*Please get me the element at position 1!*

In Ruby, you can do this with square brackets like so:

```ruby
words = ["one", "two", "three"]
puts words[1]
```

`words[1]` means: from the array `words` get the element at position
`1`. `puts` will then print this value out to the screen. (`puts` stands for
"(out-) put string".)

Funnily, this will print out `two`, and not `one`.

Huh? The reason for this is: The first position in an array is 0, not 1. So the
position 1 refers to the second element, not the first one.

In programming books and the Ruby documentation you'll often find the word
"index" to be used instead of "position" in this context.

In order to add an element to an existing array you can use the operator `<<`,
called "shovel" operator, like so:

```ruby
words = ["one", "two", "three"]
words << "four"
puts words[3]
```

This prints out `four`: The string `"four"` has been "shoveled" into, that
means, appended to the array. And since it now sits at position `3` we can
access it using `words[3]`.

You can also set an element to a specific index, like so:

```ruby
words = ["one", "two", "three"]
words[3] = "four"
puts words[3]
```

This also prints out `four`.

On formatting: Note that there are no spaces inside the square brackets,
and there's one space after each comma.

Exercises: Now would be a good time to do some of the [exercises on
arrays](/16-exercises/03-arrays_1.html).
