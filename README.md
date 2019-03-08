# Math Operators in Ruby

## Learning Goals

- Recognize `+` as the symbol for addition
- Demonstrate the addition operator
- Recognize `-` as the symbol for subtraction
- Demonstrate the subtraction operator
- Recognize `*` as the symbol for multiplication
- Demonstrate the multiplication operator
- Recognize `/` as the symbol for division
- Demonstrate the division operator
- Recognize the modulo operator
- Demonstrate the modulo operator
- Recognize `Math.sqrt`
- Demonstrate `Math.sqrt`

## Introduction

Many people associate being a programmer with being a math genius. Thankfully,
this is not a requirement. In fact, during the early years of programming,
computer tasks were often conflated with low-level clerical work, like typing
or filing, even though computers were less capable of automating very complex
calculations.

However, sometimes we need to do some mathematical work. Every programming
language has numerical and math capabilities built in for ease and convenience.
Ruby includes a large and powerful set these capabilities.  There are various
math symbols in Ruby -- many of which might look familiar to you:

| symbol | name     | operation |
|--------|----------|-----------|
| `+`    | plus     | addition |
| `-`    | minus    | subtraction |
| `/`    | slash    | division |
| `*`    | asterisk | multiplication |
| `%`    | percent  | modulo |

Most of these symbols behave the same way as they do in arithmetic. We'll
explain in more detail some of these capabilities available in Ruby. A full
list of operators can be found in [Ruby docs][ref].

## Recognize `+` as the Symbol for Addition

Addition's symbol should look familiar. The symbol that is used to perform this
operation is (`+`).

## Demonstrate the Addition Operator

To get a feel for performing addition operations in Ruby, let's experiment. Open
up IRB by opening your terminal; type `irb` and hit enter and type the commands
below:

```ruby
10 + 1 #=> 11
```

```ruby
5 + -1 #=> 4
```

In order to exit IRB, type `exit` and hit enter/return **or** `control + c`.

## Recognize `-` as the Symbol for Subtraction

Like addition, the symbol for subtraction (`-`) is also the same as in common
arithmetic.

## Demonstrate the Subtraction Operator

Let's experiment again. Open IRB and type these commands below:

```ruby
4 - 13 #=> -9
```

```ruby
11 - -11 #=> 22
```

## Recognize `*` as the Symbol For Multiplication

The symbol for the multiplication (`*`) might look a little different
than how we would write it on paper. Programming uses `*` so that we don't
confuse it with the letter `x`.

## Demonstrate the Multiplication Operator

Use IRB and try typing the following the multiplication commands:

```ruby
10 * 10 #=> 100
```

```ruby
11 * -11 #=> -121
```

If everything was typed correctly, your results should be `100` and `-121`.
Nothing out of the ordinary, right?


## Recognize `/` as the Symbol For Division

The symbol for the division (`/`) is a forward slash. There's no handy `÷`
character on most keyboards, so programmers adopted `/`.

***Division behaves differently in Ruby than you might expect***

Pay attention as we demonstrate it.

## Demonstrate the Division Operator

Open up IRB and try typing the following the division commands:

```ruby
8 / 3 #=> 2
```
```ruby
4 / 13  #=> 0
```

If you tested out each one, you might notice that when dividing a number that
has a remainder, or fraction in the value, that amount is left out and the
result you're left with is a whole number. This is different from regular
arithmetic, and is a feature in programming that may feel unfamiliar.

When you type a statement like `9 / 2` into IRB, you would expect the result to
be 4.5, but what is returned is actually 4.

This is because of the _type_ of number being used. In Ruby, and most
programming languages, numbers can be _integers_, which are whole numbers, or
_floats_, which are decimal numbers.

When you divide integers (whole numbers), they will return integers without
rounding and the numbers behind the decimal is removed. When you divide floats,
you'll get floats. If you mix integers with floats, you get a float.

If you type `9.0`, you're creating a float:

```ruby
9.0 / 2 # => 4.5
```
When you divide a float, a float is returned. If you divide a float and an
integer, a float will be returned.

## Identify the Modulo Operator

Speaking of remainders from division, sometimes it's very handy to know about
the remainder. The modulo operator (`%`) will let us get that remainder amount.
It does this for _either_ integer or float division.

## Demonstrate the Modulo Operator

```ruby
5 % 2 #=> 1
5.0 % 2 => 1.0
```

It might not be clear when to use the modulo operator, however, knowing the
remainder of a division is immensely useful in certain situations, like
determining if a number is odd or even (How do those numbers' remainders differ
when divided by two?) or divisible by seven.

We've actually all likely used modular math in our lives already -- it's also
called "clock arithmetic". Have you ever had to calculate when you might arrive
at your destination after a flight or train was heavily delayed? This is a very
similar concept.

## Recognize `Math.sqrt`

As mentioned previously, Ruby provides an extensive range of math related
functions. It gives you access to mathematics tools such as square root, sine,
cosine, and tangent via Ruby methods. A full description of the `Math` module
is [here][math]. You should memorize this module name, but you need not
memorize every math function, just start research there if you need it.

To access these in your code, refer to the module `Math` and call the method on
the module like `Math.tan()` or `Math.sqrt()`.

As the name hints, `Math.sqrt()` returns the non-negative square root of any
given number.

## Demonstrate `Math.sqrt`

A square root of a number is a value that, when multiplied by itself, gives the
number. For example, `4 × 4 = 16`, so the square root of "16" is "4".

To get the square root of 9 you'd write:

```ruby
Math.sqrt(9)
#=> 3
```

[Read more about the Math module and the available methods][math]

## Conclusion

Ruby provides us with many math and arithmetic capabilities. Some look and work
identically to what we may have learned in a math class, however, there are a
few other math tricks -- like using modulo `%` to find out the remainder of a
division, and use the remainder to check if a number is divisible by another, or
the `Math` method that can help us calculate square root or round a float up or
down to the nearest whole number.

## Resources

- [Ruby Arithmetic Operators](https://www.w3resource.com/ruby/ruby-arithmetic-operators.php)
- [Ruby Docs: Math](https://ruby-doc.org/core-2.3.0/Math.html)
- [Fun With Modular Arithmetic](https://betterexplained.com/articles/fun-with-modular-arithmetic/)

[ref]: https://www.w3resource.com/ruby/ruby-arithmetic-operators.php
[math]: https://ruby-doc.org/core-2.2.0/Math.html
