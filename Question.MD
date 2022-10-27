# Short Answer Question
Author: Nicolas Matthew Suhardi (nicmatt@uw.edu)

DO NOT DISTRIBUTE!

---

## Question 1

There's a `double` variable called `someDecimal` that contains some decimal number. Explain what the code below does:

```java
System.out.println(Math.round(someDecimal * 100.0) / 100.0);
```

Explain what the code does in English!

---

## Question 2

What is the output of the following code?

(assume that `import java.util.*;` is present)

```java
Random rand = new Random();

int maxNumber = 5673;

for (int i = 1; i <= 4; i++) {
    int randNum = rand.nextInt(i) + 1;

    maxNumber = Math.max(maxNumber, randNum);
}

System.out.println(maxNumber);
```

> Write 'random' if the output is random or 'error' if the code does not compile.

---

## Question 3

What is the output of the following code?

```java
public class Demo {
    public static final int SOME_NUMBER = 13;

    public static void main(String[] args) {
        changeNumber();

        System.out.println(SOME_NUMBER);
    }

    public static void changeNumber() {
        SOME_NUMBER = 15;
    }
}
```

> Write 'random' if the output is random or 'error' if the code does not compile.

---

## Question 4

What is the output of the code below?

```java
boolean result = Math.pow(2, 3) != 8 && Math.pow(3, 2) != 9;
System.out.println(result);
```

---

## Question 5

What is the output of the code below:

```java
public class Demo {
    public static void main(String[] args) {
        int someNumber = 9;
        changeNumber(someNumber);

        System.out.println("After change: " + someNumber);
    }

    public static void changeNumber(int someNumber) {
        System.out.println("Before change: " + someNumber);
        someNumber = 4;
    }
}
```

> Write 'error' if the code does not compile.

---

## Question 6

What is the output of the code below:

```java
public class Demo {
    public static void main(String[] args) {
        int someNumber = 9;
        changeNumber(someNumber);

        System.out.println("After change: " + someNumber);
    }

    public static int changeNumber(int someNumber) {
        System.out.println("Before change: " + someNumber);
        someNumber = 4;
    }
}
```

> Write 'error' if the code does not compile.

---

## Question 7

What is the output of the code below:

```java
public class Demo {
    public static void main(String[] args) {
        int someNumber = 9;
        changeNumber(someNumber);

        System.out.println("After change: " + someNumber);
    }

    public static void changeNumber(int someNumber) {
        System.out.println("Before change: " + someNumber);
        someNumber = 4;

        return someNumber;
    }
}
```

> Write 'error' if the code does not compile.

---

## Question 8

What is the output of the code below:

```java
public class Demo {
    public static void main(String[] args) {
        int someNumber = 9;
        changeNumber(someNumber);

        System.out.println("After change: " + someNumber);
    }

    public static int changeNumber(int someNumber) {
        System.out.println("Before change: " + someNumber);
        someNumber = 4;

        return someNumber;
    }
}
```

> Write 'error' if the code does not compile.

---

## Question 9

Explain in English what the method below does:

```java
public static int workOverTime(int x, int y) {
    int result = 1;
    for (int i = 1; i <= y; i++) {
        result *= x;
    }

    return result;
}
```

> Do not mention anything about the loop in your answer. Give a brief description of what the code does instead of describing what each iteration of the loop does.

---

## Question 10

Is the two code below equivalent?

Code 1:
```java
if (!isEven) {
    System.out.println("The number is odd");
} else {
    System.out.println("The number is even");
}
```

Code 2:
```java
if (isEven == false) {
    System.out.println("The number is odd");
} else {
    System.out.println("The number is even");
}
```

---

## Question 11

Is the two code below equivalent?

Code 1:
```java
if (someNumber % 2 == 1) {
    return false;
} else {
    return true;
}
```

Code 2:
```java
return someNumber % 2 == 0;
```
---

## Question 12

What is the output of the code below:
```java
public class IfElseMystery3 {
    public static void main(String[] args) {
        mystery(40);
        mystery(0);
        mystery(12);
        mystery(20);
    }
    
    public static void mystery(int n) {
        System.out.print(n + " ");
        if (n > 10) {
            n = n / 2;
        } else {
            n = n + 7;
        }
        if (n * 2 < 25) {
            n = n + 10;
        }
        System.out.println(n);
    }
}
```

---

## Question 13

what is the output of the code below:
```java
public class ParameteryMystery3 {
    public static void main(String[] args) {
        String hear = "bad";
        String song = "good";
        String good = "hear";
        String walk = "talk";
        String talk = "feel";
        String feel = "walk";
        claim(feel, song, feel);
        claim(good, hear, song);
        claim(talk, "song", feel);
        claim("claim", talk, walk);
    }

    public static void claim(String hear, String good, String song) {
        System.out.println("to " + hear + " the " + song + " is " + good);
    }
}
```
---

## Question 14

What is the output of the following code:

```java
import java.util.*;

public class Demo {
    public static void main(String[] args) {
        Random rand = new Random();

        // Generate the first Random number
        int randNum = rand.nextInt(5) + 3;

        moreNumber(randNum, rand);
    }

    public static void moreNumber(Random randNum, int rand) {
        int otherNumber = randNum.nextInt(5) + 3;

        System.out.println(otherNumber - rand);
    }
}
```

> Write 'random' if the output is random or 'error' if the code does not compile.

---

## Question 15

What is the output of the code below:

```java
public class Demo {
    public static void main(String[] args) {
        printTwo();
        System.out.println("2");
        printThree();
        printOne();
    }

    public static void printOne() {
        System.out.println("3");
        printThree();
    }

    public static void printTwo() {
        printOne();
        System.out.println("4");
        printThree();
    }

    public static void printThree() {
        System.out.println("2");
        System.out.println("1");
    }
}
```


