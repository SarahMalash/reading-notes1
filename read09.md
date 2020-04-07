# read09
## What is functional programming?
 a programming paradigm a style of building the structure and elements of computer programs.
  *that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data*
  ## pure functions:
  1. It returns the same result if given the same arguments
  2. It does not cause any observable side effects
  *Any function that relies on a random number generator cannot be pure.*
  ## Pure functions benefits
  The code’s definitely easier to test. We don’t need to mock anything
  *When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.*

  ## Functions as first-class entities can:
1. refer to it from constants and variables
2. pass it as a parameter to other functions
3. return it as result from other functions
## Higher-order functions:
1. takes one or more functions as arguments
2. returns a function as its result
## Filter:
Given a collection, we want to filter by an attribute. The filter function expects a true or false value to determine if the element should or should not be included in the result collection.
## Map:
The map method transforms a collection by applying a function to all of its elements and building a new collection from the returned values.
## Reduce:
The idea of reduce is to receive a function and a collection, and return a value created by combining the items.