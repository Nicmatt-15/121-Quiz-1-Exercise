# Coding Questions
Author: Nicolas Matthew Suhardi (nicmatt@uw.edu)

DO NOT DISTRIBUTE!

---

## Question 1 - Methods and Parameters

Print the following output:
```
Good morning, Nicolas!
What plan do you have at 6?

Good evening, Matthew!
What plan do you have at 5?
```

Requirement:

1. You must only create 1 method (other than the main method)
2. Your main method should not have any print statement
3. You can only have a total of 2 print statement in your program.

---

## Question 2 - Conditional Structure

Given the following starter code:

```java
Random rand = new Random();
int netIncome = rand.nextInt(501) - 250;

// Your code below
```

You should print:

- `You're a big saver` if 250 < netIncome
- `You're a saver` if 0 < netIncome <= 250
- `You're a spender` if -250 < netIncome <= 0
- `You're a big spender` if netIncome <= -250

Requirement:
- You may not use && or || operator
- You may not use nested if/else if/else

---

## Question 3 - Scalable Figures

Given the starter code below:

```java
public class Demo {
    public static final int SIZE = 3;

    public static void main(String[] args) {

    }
}
```

That produce the following output when `SIZE = 3`:

```
#============#
|    <><>    |
|  <>....<>  |
|<>........<>|
|<>........<>|
|  <>....<>  |
|    <><>    |
#============#
```

and the following output when `SIZE = 4`:

```
#================#
|      <><>      |
|    <>....<>    |
|  <>........<>  |
|<>............<>|
|<>............<>|
|  <>........<>  |
|    <>....<>    |
|      <><>      |
#================#
```

Complete the starter code above!

Requirement:
- Your code should produce the scalable figure above where if the value of `SIZE` is changed, the figure automatically scales.
- You can write all your code in the main method

---

## Question 4 - Implementing `.indexOf(...)`

Given the following starter code:

```java
String sentence = "I like CSE 121";
String letter = "1";

// Your code here
```

Write a code that prints out the smallest index of where the letter appears in the sentence (and -1 if the letter is not found).

Requirement:
- You may not use the indexOf method
- You must use exactly one for-loop

---

## Question 5 - Undouble

Given the starter code:
```java
public class Undouble {
    public static void main(String[] args) {
        Scanner console = new Scanner(System.in);
        System.out.println(undouble("odegaard"));
        System.out.println(undouble("baz"));
        System.out.println(undouble("mississippi"));
        System.out.println(undouble("carry"));
        System.out.println(undouble("juggle"));
        System.out.println(undouble("")); // expect blank line
        System.out.println(undouble("oops"));
        System.out.println(undouble("foobar"));
        System.out.println(undouble("apple"));
        System.out.println(undouble("berry"));
        System.out.println(undouble("theses"));
        System.out.println(undouble("little"));
    }

    // TODO: Your Code Here -> Write a method
    // called undouble for this problem
}
```

Write a static method called `undouble` that takes a String as a parameter and that returns a new String obtained by replacing every pair of repeated adjacent letters with one of that letter.

For example, the String "bookkeeper" has three repeated adjacent letters ("oo", "kk", and "ee"), so undouble("bookkeeper") should return the String "bokeper".

> You may assume that the string is composed entirely of lowercase letters. 
> 
> The method might also be passed an empty String `""`, in which case it  returns an empty String.

---

## Question 6 - Quadrant

Given the following starter code:
```java
public class Quadrant {
    public static void main(String[] args) {
        findQuadrant(0, 5);
        findQuadrant(0, 0);
        findQuadrant(7, 3);
        findQuadrant(-1, 4);
        findQuadrant(-5, 0);
        findQuadrant(-7, -4);
        findQuadrant(3, -2);
    }

    // Write the method findQuadrant below
}
```

Write a static method called `findQuadrant` that takes in two `int` (`x` and `y`) representing a coordinate point. The method will then find in which quadrant the coordinate point lies.

The rule is as follow:
1. The method should print out the String `Quadrant I` if both the `x` and `y` coordinate are positive.
2. The method should print out the String `Quadrant II` if the `x` coordinate is negative and the `y` coordinate is positive.
3. The method should print out the String `Quadrant III` if both the `x` and `y` coordinate are negative.
4. The method should print out the String `Quadrant IV` if the `x` coordinate is positive and the `y` coordinate is negative.
5. The method should print out `x axis` if the `y` value is 0.
6. The method should print out the `y axis` if the `x` value is 0.

Requirement:
- You may use nested conditional
- You may also use the && and || operator

---

## Question 7 - Implementing `.trim()`

In Java, String has a method called `.trim()` that removes all leading
and trailing spaces from a String.

Example:
```java
String someText = "  some  space, eh?  ";
System.out.println(someText.trim());
```

Output:
```
some  space, eh?
```

> Notice that .trim() only removes the spaces before the first letter and the space after the very last letter.

Our goal is now to implement this method ourselves!

You are given the following starting code (with instruction in the code)!
```java
public class Demo {
    public static void main(String[] args) {
        System.out.println(trim("  "));
        System.out.println(trim("  hello"));
        System.out.println(trim("hello   "));
        System.out.println(trim("  hello  "));
        System.out.println(trim("   multi   word "));
        System.out.println(trim(""));
    }

    // Write a method called trim that takes in
    // a String and returns back the String stripped
    // of its leading and trailing spaces
}
```

Requirements:
1. You may not use the `trim()` String method (for obvious reason :sweat_smile:)
2. Your method should not have extra parameter