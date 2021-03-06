# New Math Notation

New symbolic representation using base 6.

## How to read it?

Each symbol consists of a left and right side, translating into two heximal digits. Once you can read the right side, you will be able to read the left side.

Broken down, here are the symbol side meanings:

![Heximal Breakdown](heximal-breakdown.png)

Basically, the two digits are glued together. To see what one side looks like on its own, you have to set the other side to one.

Notice, the digit *4* contains the symbol for divisible by 2.

Notice, the digit *0* contains the symbol for divisible by 2 and 3.

Finally, notice all digits contain the symbol for divisible by 1.

Hence, by looking at the symbol, it is very easy to determine if it is divisible by 2, 3, or 10 base 6.

If you want to see what any digit looks like by itself, you'd have to set the other digit to 1.

If you are wondering why *0* is so complicated looking, understand that this is simply implying that zero is even, and also divides 3. Of course 0 would divide all numbers, but from the perspective of the heximal number system, the equivalent number of *6* ends up dividing 2 and 3, so that ends up being the definition for *0*.

*5* is not divisible by 2 or 3. So it needed a symbol of its own. Since it's the only other prime, and - and \ were already used to represent the other primes, I used / for this last prime.

For *4*, Since it's divisible by 2, I had to include the -. To represent *4*, I wanted to say something like "double the 2". So my way of doing that was to write - twice, hence =.

Finally, why doesn't *0* contains symbols for 4 or 5?

That is because *0* is meant to be used to represent a multiple of six. "10" equals 6. "20" equals 12, "30" equals 18, etc.

2 and 3 will *always* divide *10* or *20* or any other *X0*. 4 and 5 will only divide some specific cases, like *40* and *50*. Since they are only exceptions, they don't influence how 0 looks like.

Now that you know how to read it, here is a handwritten list of numbers / symbols:

![heximal](heximal.jpg)

Please let me know if this looks confusing, and I will be happy to talk more about it with you.

I tried to find unicode character equivalents, I found a few here:

### 11: ˡ
### 22: ⫠
### 33: 人
### 44: ⫨
### 55: ⩛
### 00: 大

## Why do this at all?

The output of mathematical formula can be considered as elegant and beautiful.

However, the mathematical notation used to describe the formula, is not elegant, and is rather arbitrary.

Frequently when mathematicians needed to invent some constant or function, they were not very creative.

For example if you look at the number *4*, there is no particular quality about that number that describes its quantity at all. In school, you just have to memorize that that's what a 4 looks like.

Similarly, check out *x*^*y* = *z*. If you want to solve for *x*, you end up with this: *y* = **ln**(*z*) / **ln**(*x*)

This is very inconsistent.. an equation which a superscript value gets solved by dividing two functions.

This inconsistency and arbitrariness causes confusion for students learning mathematics.

I intend to completely redefine all of mathematics to feel more intuitive and consistent.

## Base

### Decimal

The decimal base prioritizes numbers 2 and 5 for easy math calculations.

It has been used mainly because of the number of fingers on our hands.

However it is not the best system to use.

### Heximal

Based on my findings from [here](https://github.com/veniamin-ilmer/better-standards/tree/master/base-6), base 6 is the most optimal base for humans to use.

It prioritizes numbers 2 and 3 for each math calculations. This is better than decimal because both 2 and 3 are within our subitizing range, making it much easier to count things in 2s and 3s.

## Grouping

When choosing the most optimal base, there are two different factors at play:

1. The base should be small enough that it is easy to remember and reuse.
2. The base should be big enough that large numbers can be represented without much difficulty.

### Decimal

In decimal, we handle this by using digits *0* to *9*, but loosly grouping numbers in 2 or 3 digits.

The number *12345* would typically be represented as *12,345*. The comma is added as a delimiter for readability, but is optional.

When reading the number out loud, it could be read in multiple different ways:

* One, Two, Three, Four, Five
* One, Twenty-Three, Forty-Five
* Twelve Thousand, Three Hundred, Forty-Five

I feel that the multiple representations of the same number causes misunderstandings.

I feel there should be one obvious way for numbers to be read.

The number "*100*" is looked at favorably as a "maximum" number, and hence we have a concept of a "percentage", where you can score an "*86%*" on a test, or get a coupon with a "*15%*" discount.

This is a lot of inconsistent from the grouping of 3 digits at a time. Why don't percentages have *1000%* as a maximum?

Also, if we are absolutely certain that the number will only be from 0 to 100, why don't we 0% as 000%? 

When expressing time, why would you write it as *4:08*? Why don't you say that the time is *4:8*? Alternatively, why don't you say that the time is *04:08*?

Same with dates. What date is this: *03-04-09*? What about *5/4/08*?

It might seem trivial, but from a software engineer's perspective, that inconsistency in spacing is a prominent cause of various bugs and extra inefficent code.

It is especially an issue for graphical design. Instead of having a fixed width, the text field has to take into account 3 different sizes, making sure object overlap doesn't happen for the different fonts used.

### Heximal

My notation system fixes issues noted above, by forcing the user into grouping it into 2 digits all the time.

It is not possible to have a separate digit. If you want to say "1, 2, 3", you will be forced into saying either "01, 02, 03" or "01, 23". You must pick which one it will be.

This grouping is consistent everywhere.

What time is it? The hours, minutes, and seconds are from 00 to 55 base 6.

Want to express a percentage? It will range from 00% to 55%

How many days are there in a month? That's right, it's from 00 to 55.

But, we are just getting started here. People are good at remembering symbols, but are limited to how many they can remember.

Generally, that quantity is known to be a maximum of 7 numbers. Hence a phone number, without the area code, is bearily memorable.

The way my notation fixes this is by merging the two numbers into one symbol. 7 decimal digits ends up being only 5 of my merged hex digits. 10 decimal digits (that includes the area code), ends up being only 6 merged hex digits.
