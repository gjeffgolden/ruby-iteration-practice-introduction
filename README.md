# Array Iteration

To iterate, defined broadly, is to repeat a process.
A political candidate might iterate over the same speech to
different crowds every night. A grocery store cashier 
iterates over a basket of grocery items, scanning each
item using the same process. Given a stack of paper, _you_
could perform an iterative process and turn that stack of
paper into a pile of paper airplanes.

In programming, we can iterate over arrays in a similar 
fashion - for every element in an array, perform some sort
of process. Iterating over arrays has many uses, including:

* Reading each element and finding the first element that matches
  some criteria we've set. _Example: given an array of
  numbers, find the biggest number._
* Reading each element and collecting _all_ elements that match
  some criteria we've set. _Example: given an array of
  numbers, find all numbers bigger than x._
* Transforming each element into something new. _Example: given
  an array of words, add 's' to the end of each._
* Reducing the elements to an aggregate value. _Example: given
  an array of prices, add each element to a total._

One of the key advantages of using iteration to work with arrays
is that we do not need to know how many elements are in the array -
we just need to write a process that will be applied to _each element_.
This becomes extremely useful for writing more abstract code. 

Imagine a teacher who wants to print out a list of student names for
attendance every day. They could write a program that hard codes each name 
to be printed - but then this program would only be useful for one
classroom. 

```ruby
puts "Sally B"
puts "Tommy H"
puts "Julia S"
puts "Pete B"
```

Alternatively, the teacher could write a program that prints
out all elements in an array instead, and just store student names in an
array. 

```ruby
students = ["Sally B", "Tommy H", "Julia S", "Pete B"]

students.each do |student|
  puts student
end
```

Here, the process has been separated away from the data. The teacher can add
students to the array and not change the code that handles printing. The
teacher could now have _many_ arrays of students and use this one program
to print out attendance sheets for all their classes!

Ruby has a few different tools we can use to handle these
tasks. In this section, we're going to look at some of these tools
and how they can help us work with arrays. Topics in this section include:

* A review of iterators
* Using each vs collect
* Transforming arrays into new arrays
* Selecting elements from arrays
* Sorting elements in arrays

In addition, here are some resources you may find helpful:

* [Ruby Iteration Primer](https://rubymonk.com/learning/books/1-ruby-primer/chapters/1-arrays/lessons/3-arrays-iteration)
* [Types of Iterators](https://www.geeksforgeeks.org/ruby-types-of-iterators/)
