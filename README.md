# Build a Calculator

## Learning Goals

- Practice doing basic math in Ruby
- Demonstrate how division in Ruby differs from normal division
- Demonstrate the modulo operator
- Play with the `Math` module
- Create appropriate behavior for methods

## Introduction

Every programming language has numbers and math capabilities built in. Ruby
includes a large and powerful set these capabilities. Do not worry if you do not
think you are great with math. There are various math symbols in Ruby -- many of
which might look familiar to you:

`+` plus `-` minus `/` slash `*` asterisk `%` percent or modulo `<`less-than `>`
greater-than `<=` less-than-equal `>=` greater-than-equal

Most of these symbols behave the same way as they do in arithmetic. We'll go in
depth on some of the additional capabilities available in Ruby.

## Practice Doing Basic Math in Ruby

One of the most basic is the capability to do simple arithmetic. Open up IRB
(open your terminal then type `irb` and hit enter) and type the commands below:
* 1 + 1
* 1 * 3
* Math.sqrt(81)
* 9 ** 2

### Order of Operations 

Enclosing an expression in parentheses `()` defines an order of operations, like
you would [expect](http://en.wikipedia.org/wiki/Order_of_operations).

* `98 + 59/13 * 8 * -5 = -62`
* `98 + (59/(13*8)) * -5 = 98`

## Demonstrate How Division in Ruby Differs From Normal Division

Type `9 / 2`. You would expect the result to be 4.5, but it's actually 4. This
is because of the type of number you are using. In Ruby, and most programming
languages, numbers can be integers (whole numbers), or floats(decimal numbers).
When you divide  integers, they return integers without rounding. The decimal is
just removed. If you type 9.0, you're creating a float, so  `9.0 / 2.0 = 4.5`.
Numbers with decimals are called floats and when you divide floats a float is
returned. If you divide a float and an integer, a float will be returned, so
`9.0/2 = 4.5`.

## Demonstrate the Modulo Operator

There is another operator that is really useful in programming. It's the modulo,
and it's represented with the percent sign `%`. The modulo operator gives you
the remainder of a number divided by another number. So `5 % 3 = 2`.

## Play With the `Math` Module

As mentioned previously, Ruby provides an extensive range of math related
functions.

Ruby has built-in methods for common math functions. The basic trigonometric and
transcendental functions are available in the [Math module](http://ruby-doc.org/core-2.2.0/Math.html).
This gives you access to mathematic tools such as square root, sine, cosine, and
tangent via Ruby methods. To access these in your code simply refer to the
module `Math` and call the method on the module. For example, to get the square
root of 9 you'd write
`Math.sqrt(9)`. [Read more about the Math module and the available methods.](http://ruby-doc.org/core-2.2.0/Math.html)

## Create Appropriate Behavior For Methods

Fork and clone this repo and open `lib/math.rb`. You'll find a bunch of empty
methods that take numbers as arguments. Build the appropriate behavior for each
of the following methods:
- addition
- subtraction
- multiplication
- division
- modulo
- square root
- order of operation

The lab is test driven, so get the tests to pass.

## Conclusion

Ruby provides us with many math and arithmetic capabilities. Some look and work
identically to what we may have learned in a math class, however, there are a
few other math tricks -- like using modulo `%` to find out the remainder of a
division, and use the remainder to check if a number is divisible by another, or
the `Math` method that can help us calculate square root or round a float up or
down to the nearest whole number.

## Resources
