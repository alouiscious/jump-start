# Practice problems

_JumpStart: Lesson 9_

## Overview

Complete each section by hand, then check your answers using `irb`

## Variables and assignment practice

```ruby
x = 5
# what value does x now hold?

z = "Hello"
# what value does z now hold?

a = 5
b = 3.2
c = a + b
# what values does c now hold?

var1 = "lawl"
var2 = "brb"
# what value does var2 now hold?

e = 6 + 3
# what values does e now hold?

f = 3.5
f = f + 2
# what value does f now hold?

poodle = 4
pitbull = 3
# what value does boxer now hold?

h = 5
h = h + h
# what values does h now hold?

j = 1
k = 2
m = 3
n = j + k + m
# what value does n now hold?

l = "moo"
q = "quack"
l  = q
# what value does l now hold?

r = "moo"
s = "quack"
t = "woof"
r = t
# what value does r now hold?

u = 5
u = u * 2
u = u * 2
u = u * 2
# what value does u now hold?

v = "b"
z = "a"
# what value does v now hold?


aa = 3234
bb = 2398
cc = 0
dd = (aa + bb) / cc
# what value does dd now hold?

yy = 7
zz = yy % 2
# what value does zz now hold?

ee = 12
ff = ee % 4
# what value does ff now hold?


zz = 17
hh = zz % 3
# what value does hh now hold?
```

## Operators practice

Consider the following variable assignments and then fill in the tables

```ruby
d = 10
e = 5.0
f = 2
g = 11.0
h = 3
i = 1.5
```

| Operation | Result | Data type of result |
| :---: | :---:| :---: |
| `d + e` |15.0 | float|
| `f + h` |5 | int|
| `g + h` | 14.0| float|
| `d - f` |8 |int |
| `g - e` | 6.0| float|
| `(h + i) - f` | 2.5|float |
| `(d - f) + e` | 13.0| float|
| `d * f` |20 | int fix| |
| `g * i` |16.5 | float| |
| `f * g` |22.0 | float| |
| `d / f` | 5| | int|
| `d / e` | 2.0| |float |
| `e / f` |2.5 | | float|
| `(g * f) / f` | 11.0| | float|
| `(d / f) * e` |25.0 | |float |
| `21 / 5` |4 | | intfixed|
| 14 / 5 |2 | |int |
| 10 % 3 | 1| |int |
| 20 % 2 |0 | | int|
| 4 % 5 | 4| | int|
| 8 % 1 |0 | | int|

## String practice

Determine the output for each of the following problems on your own and then check your answer using `irb`

```ruby
# problem 1
my_string = "I love Seattle"
my_string.slice(7)

# problem 2
my_string = "I love Seattle"
my_string.slice(2, 4)

# problem 3
my_string = "I love Seattle"
my_string.slice("Seattle")

# problem 4
my_string = "Ada"
my_string += " Lovelace"

# problem 5
my_string = "Ada"
my_string << " codes" << " it!"

# problem 6
my_string = "Ada"
my_string.concat(" likes to code").slice(4...9)

# problem 7
my_string = "Hello world"
"Goodbye " + my_string.slice(6, 5) << "!"

# problem 8
my_string = "Hello world!"
my_string.slice(0...5).concat(", goodbye!")

# problem 9
my_string = "Hello world!"
my_string.slice(0) << "i" + "!"

# problem 10
my_string = "I love Ruby"
my_string.slice(7, 4).concat(my_string.slice(2..5)) + my_string.slice(0)

# problem 11
my_string = "I love Ruby"
my_string.slice(7, 4).concat(my_string.slice(2...6)) + my_string.slice(0)

# problem 12
my_string = "I love Ruby"
"R".concat(my_string.slice(8, 3) + " rocks!")

# problem 13
my_string = "I love Ruby"
my_string.slice(2, 4) << my_string.slice(7...11).concat(my_string.slice(2...6))
```
Practice Problem Answers

 my_string="I love Seatle"
=> "I love Seatle"
irb(main):002:0> my_string.slice(7)
=> "S"
irb(main):003:0> my_string="I love Seattle"
=> "I love Seattle"
irb(main):004:0> my_string.slice(7)
=> "S"
irb(main):005:0> my_string.slice(2,4)
=> "love"
irb(main):006:0> my_string.slice(2, 4)
=> "love"
irb(main):007:0> my_string.slice("Seattle")
=> "Seattle"
irb(main):008:0> my_string = "Ada"
=> "Ada"
irb(main):009:0> my_string +=" Lovelace"
=> "Ada Lovelace"
irb(main):010:0> my_string +=" Lovelace"
=> "Ada Lovelace Lovelace"
irb(main):011:0> my_string = "Ada"
=> "Ada"
irb(main):012:0> my_string << " codes" << " it!"
=> "Ada codes it!"
irb(main):013:0> my_string = "Ada"
=> "Ada"
irb(main):014:0> my_string.concat(" like to code.").slice(4...9)
=> "like "
irb(main):015:0> my_string.concat(" likes to code.").slice(4...9)
=> "like "
irb(main):016:0> my_string.concat(" likes to code.").slice(4...10)
=> "like t"
irb(main):017:0> my_string.concat(" likes to code.")
=> "Ada like to code. likes to code. likes to code. likes to code."
irb(main):018:0> my_string = "Hello, World!" 
=> "Hello, World!"
irb(main):019:0> "Goodbye " + my_string.slice(6, 5) << "!"
=> "Goodbye  Worl!"
irb(main):020:0> my_string = "Hello world!"         
=> "Hello world!"
irb(main):021:0> "Goodbye " + my_string.slice(6, 5) << "!"
=> "Goodbye world!"
irb(main):022:0> my_string = "Hello world!"
=> "Hello world!"
irb(main):023:0> my_string.slice(0...5).concat(",goodbye!")
=> "Hello,goodbye!"
irb(main):024:0> my_string.slice(0...5).concat(", goodbye!")
=> "Hello, goodbye!"
irb(main):025:0> my_string = "Hello world!"
=> "Hello world!"
irb(main):026:0> my_string.slice(0) << "i" + "!"
=> "Hi!"
irb(main):027:0> my_string = "I love Ruby"
=> "I love Ruby"
irb(main):028:0> my_string.slice(7, 4).concat (my_string.slice(2...6)) + my_string.slice(0)
=> "RubyloveI"
irb(main):029:0> my_string = "I love Ruby"
=> "I love Ruby"
irb(main):030:0> "R".concat(my_string.slice(8, 3) + "rocks!")
=> "Rubyrocks!"
irb(main):031:0> my_string = "I love Ruby"           => "I love Ruby"
irb(main):032:0> "R".concat(my_string.slice(8, 3) + " rocks!")
=> "Ruby rocks!"
irb(main):033:0> my_string = "I love Ruby"           => "I love Ruby"