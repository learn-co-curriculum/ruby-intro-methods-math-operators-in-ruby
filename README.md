# Build a Calculator

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

Many people might associate being a programmer with being a math genius. In
reality, this is not a requirement. Ironically, during the early years of
programming, computer tasks were often conflated with low-level clerical work,
like typing or filing, even though computers were less capable of automating
very complex calculations at the time.

However, sometimes we need to do some mathematical work. Every programming
language has numbers and math capabilities built in for ease and convenience.
Ruby includes a large and powerful set these capabilities.  There are various
math symbols in Ruby -- many of which might look familiar to you:

| symbol | name | operation |
| `+` | plus | addition |
| `-` | minus | subtraction |
| `/` | slash | division |
| `*` | asterisk | multiplication |
| `%` | percent | modulo |

Most of these symbols behave the same way as they do in arithmetic. We'll
explain in more detail some of these capabilities available in Ruby. A full list
of operators can be found in [Ruby docs](https://www.w3resource.com/ruby/ruby-arithmetic-operators.php).

## Recognize `+` as the Symbol for Addition

No matter where you may have received your education, addition is a universal
concept that will look familiar; the symbol that is used to perform this
operation (`+`) also looks exactly the same as we've seen it before.

## Demonstrate the Addition Operator

To get a feel for performing addition operations in Ruby, let's experiment. Open
up IRB by opening your terminal; type `irb` and hit enter and type the commands
below:

```ruby
10 + 1
```

```ruby
5 + -1
```

Works just as expected, yes? In order to exit IRB, type `exit` and hit
enter/return or `control + z` on a Mac.

## Recognize `-` as the Symbol for Subtraction

Like addition, the symbol for subtraction (`-`) is also the same as in common
arithmetic. 

## Demonstrate the Subtraction Operator

Let's experiment again. Open IRB and type these commands below:

```ruby
4 - 13
```

```ruby
11 - -11
```

As you can see, Ruby can perform any operation that a simple calculator can!

## Recognize `*` as the Symbol For Multiplication

The symbol for the multiplication (`*`) might look a little different
than how we would write it on paper, but again, like a calculator, the same
operations can be performed and we will get the same results as if it were
performed by hand.

## Demonstrate the Multiplication Operator

Use IRB and try typing the following the multiplication commands:

```ruby
10 * 10
```

```ruby
11 * -11
```

If everything was typed correctly, your results should be "100" and "-121".
Nothing out of the ordinary, right?


## Recognize `/` as the Symbol For Division

The symbol for the division (`/`) is a forward slash. This may differ from
writing common arithmetic as well and is not the only difference you'll notice.

## Demonstrate the Division Operator

Open up IRB and try typing the following the division commands:

```ruby
8 / 3
```
```ruby
4 / 13
```

If you tested out each one, you might notice that when dividing a number that
has a remainder, or fraction in the value, that amount is left out and the
result you're left with is a whole number. This is different from regular
arithmetic, and is a feature in programming that may feel unfamiliar.

When you type an a statement like `9 / 2` into IRB, you would expect the result
to be 4.5, but what is returned is actually 4. This is because of the type of
number being used. In Ruby, and most programming languages, numbers can be
_integers_, which are whole numbers, or _floats_, which are decimal numbers.
When you divide integers (whole numbers), they will return integers without
rounding and the numbers behind the decimal is removed. If you type `9.0`,
you're creating a float:

```ruby
9.0 / 2
# => 4.5
```
When you divide a float, a float is returned. If you divide a float and an
integer, a float will be returned.

## Identify the Modulo Operator

Modulo (abbreviated "mod"), represented by the `%` symbol, is the operator that
computes the _remainder_ after integer division. As we demonstrated previously,
when two integers are divided and the result is not a whole number, the result
given is a known as the "quotient", therefor the numbers behind the decimal are
excluded. 

## Demonstrate the Modulo Operator

To briefly recap, the modulo operator computes the _remainder_ after division,
specifically with _integers_.

For example, 15 is evenly divisible by 3, so "0" would be the remainder when you
divide 15 by 3. However, if we divide `12 / 10` we get a quotient of "1" and a
remainder of "2":

```ruby
12 / 10
# => 1 (quotient)
```

The remainder for this operation would be "2" if we could see the full number.
If we perform the same operation using the modulo operator, our result that
would also be "2".

```ruby
12 % 10
# => 2
```

It might not be clear when to use the modulo operator, however, knowing the
remainder of a division is immensely useful in certain situations, like
determining if a number is odd or even or divisible by seven.

We've actually all likely used modular math in our lives already -- it's also
called "clock arithmetic". Have you ever had to calculate when you might arrive
at your destination after a flight or train was heavily delayed? This is a very
similar concept.

## Recognize `Math.sqrt`

As mentioned previously, Ruby provides an extensive range of math related
functions. It gives you access to mathematic tools such as square root, sine,
cosine, and tangent via Ruby methods. To access these in your code, refer to the
module `Math` and call the method on the module.

The `Math.sqrt()` method exists in library of Ruby. The purpose of this method
is to obtain the non-negative square root of any given number.

## Demonstrate `Math.sqrt`

A square root of a number is a value that, when multiplied by itself, gives the
number. For example, `4 × 4 = 16`, so the square root of "16" is "4".

To get the square root of 9 you'd write:

```ruby
Math.sqrt(9)
#=> 3
```

Alternatively, you can check by multiplying the result against itself.

```ruby
3 * 3
#=> 9
```

[Read more about the Math module and the available methods](http://ruby-doc.org/core-2.2.0/Math.html)

## Conclusion

Ruby provides us with many math and arithmetic capabilities. Some look and work
identically to what we may have learned in a math class, however, there are a
few other math tricks -- like using modulo `%` to find out the remainder of a
division, and use the remainder to check if a number is divisible by another, or
the `Math` method that can help us calculate square root or round a float up or
down to the nearest whole number.

## Resources

[Ruby Arithmetic Operators](https://www.w3resource.com/ruby/ruby-arithmetic-operators.php)
[Ruby Docs: Math](https://ruby-doc.org/core-2.3.0/Math.html)
[Fun With Modular Arithmetic](https://betterexplained.com/articles/fun-with-modular-arithmetic/)