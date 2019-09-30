# Loops Lab

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link of your Fork on Canvas and submit


## Question 1

Write code that prints all the numbers from 1 to 150, **inclusive.**
/*ANSWER

for numbers in 1...150 {
    print(numbers)
}

*/
***
## Question 2

Write code that prints all the numbers from 142 to 159, **exclusive.**

/*ANSWER
for numbers in 142..<159 {
    print(numbers)
}

*/

***
## Question 3

Write code that prints only the even numbers from 15 to 80, **inclusive.**

/*ANSWER

for numbers in 15...80 {
    if numbers % 2 == 0{
        print(numbers)
    }
}
*/

***
## Question 4

Write code that prints only the odd numbers from 19 to 51, **inclusive.**

/*ANSWER
for numbers in 19...51 {
    if numbers % 2 == 1{
        print(numbers)
    }
}
*/

***
## Question 5

Write code that prints all the numbers that end in a **5** from 1 to 100, **exclusive.**

/*ANSWER
for numbers in 1..<100 {
    if numbers % 10 == 5{
        print(numbers)
    }
}
*/
***
## Question 6

Write code that prints all the numbers that end in a 7 from 1 to 40, **inclusive.**

/*ANSWER
for numbers in 1...40 {
    if numbers % 10 == 7 {
        print(numbers)
    }
}
*/

***
## Question 7

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 3`

***
/*ANSWER
for numbers in 20...150 where numbers % 3 == 0 {
    print(numbers)
}
*/
## Question 8

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 2 and 3`

***
/*ANSWER
for numbers in 20...150 where numbers % 3 == 0 && numbers % 2 == 0 {
    print(numbers)
}
*/
## Question 9

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that end with a 4`

***
/*ANSWERS
for numbers in 20...150 where numbers % 10 == 4 {
    print(numbers)
}
*/
## Question 10

Given a range of numbers from 20 to 150, print out all the numbers that follows these conditions:

`Print out numbers: 31, 35, 40 to 60.`

***
/*ANSWER
for numbers in 20...150 where numbers == 31 || numbers == 35 || numbers >= 40 && numbers <= 60 {
    print(numbers)
}
*/
## Question 11

Without using Xcode, how many times will the loop below run?  Explain why.

```swift
var i = 5

while (i > 3) {
    i += 1
}

// Your explanation here
```
/*
This code will run an infinite amount of times.

*/

***
## Question 12

Change the code below to make the loop stop executing when i reaches 9.

```swift
var i = 5

while (i > 3) {
    i += 1
}
```
/*ANSWER
var i = 5

while (i < 9) {
    i += 1
    print(i)
}
*/
***
## Question 13

Change the code below to make the loop stop executing after it has run 1,000 times.

```swift
var i = 5

while (i > 3) {
    i += 1
}
```
/*ANSWER
var i = 5

while (i < 1005) {
    i += 1
    print(i)
}
*/
***
## Question 14

Change the code below to make the loop stop executing after it has run 1,000 times and also make it print out the current value of i **only if i is an even number.**

```swift
var i = 5

while (i > 3) {
    i += 1
}
```
/*ANSWER
var i = 5

while (i < 1005) {
    i += 1
    if i % 2 == 0{
        print(i)
    }
}
*/

***
## Question 15

What's the difference in syntax between the following two while loops?  Will their outputs be different?  Explain why or why not.

```swift
var i = 1
//loop one
while i <= 10 {
    print("i = \(i)")
    i += 1
}

//loop two
var i = 1

repeat {
    print("i = \(i)")
    i += 1
} while i <= 10
```
/*ANSWER 
They will print out the same number because both loops end when they reach the number 10. 
*/
# Bonus =)

***
## Question 1

What's the difference between `break` and `continue`?  Give an example that demonstrates their differences.
/*ANSWER
Break - breaks loop and stops searching for other conditions
Continue - continue onto the next value/condition

*/
***
## Question 2

Without using Xcode, what will the loop below print? Select all that apply.

```swift
for i in 1...10 {
    if (i >= 4 && i <= 7){
        continue
    }
    print(i)
}
```

[x]1
[x]2
[x]3
[]4
[]5
[]6
[]7
[x]8
[x]9
[x]10

***
## Question 3

Without using Xcode, what will the loop below print? Select all that apply.

```swift
for i in 1...10 {
    if (i >= 4 && i <= 7){
        break
    }
    print(i)
}
```

[x]1
[x]2
[x]3
[]4
[]5
[]6
[]7
[]8
[]9
[]10

***
## Question 4

Without using Xcode, what will the loop below print?  Explain below.

```swift
outerloop: for x in 1...3 {
    innerloop: for y in 1...3 {
        if y == 2{
            continue outerloop
        }
        print("x = \(x), y = \(y)")
    }
}
```
***
## Question 5

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** x and y are both integers.



***
## Question 6

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** the difference of x and y is at least 5, and x and y are both integers.

***
## Question 7

Print the first `N` square numbers. A **square number**, also called perfect square, is an integer that is obtained by squaring some other integer; in other words, it is the product of some integer with itself (ex. 1 = 1*1, 4 = 2 * 2, 9 = 3* 3 …).

Example:
Input: `var N = 5`

Output:
```swift
1
4
9
16
25
```

***
## Question 8

Given an integer N draw a square of N x N asterisks. Look at the examples.

Example 1:
Input: `var N = 2`

Output:
```swift
**
**
```

Example 2:
Input: `var N = 3`

Output:
```swift
***
***
***
```

Hint 1
Try printing a single line of * first.

Hint 2
You can use print("") to print an empty line.

***
