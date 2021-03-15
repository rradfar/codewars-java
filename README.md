![java](images/java-logo.png)

# [Codewars](https://www.codewars.com/) Java Solutions

## Challenges

|  Kyu  | Questions                                   |
| :---: | :------------------------------------------ |
|   8   | [Beginner Series #2 Clock](#beginner-series-2-clock)               |
|   8   | [Century From Year](#century-from-year)               |
|   8   | [Even or Odd](#even-or-odd)                 |
|   6   | [Find the Odd Int](#find-the-odd-int)                 |
|   8   | [Is n Divisible by x and y?](#is-n-divisible-by-x-and-y)               |
|   8   | [Keep Hydrated!](#keep-hydrated)                 |
|   6   | [Multiples of 3 or 5](#multiples-of-3-or-5) |
|   8   | [Multiply](#multiply)                       |
|   7   | [Vowel Count](#vowel-count)                 |

---

## Beginner Series #2 Clock

The clock shows h hours (0 <= h <= 23), m minutes (0 <= m <= 59) and s seconds (0 <= s <= 59) after midnight. Your task is to write a function which returns the time since midnight in milliseconds.

Examples:

```
h = 0, m = 0, s = 0 -> res = 0
h = 0, m = 1, s = 1 -> res = 61000
h = 1, m = 0, s = 1 -> res = 3601000
```

```java
public class Clock {
  public static int Past(int h, int m, int s) {
    // Your solution
  }
}
```

<details><summary>Solution</summary>

```java
public class Clock {
  public static int Past(int h, int m, int s) {
    return ((h * 60 * 60) + (m * 60) + s) * 1000;
  }
}
```
</details>

---

**[⬆ Back to Top](#challenges)**

## Century From Year

The first century spans from the year 1 up to and including the year 100, The second - from the year 101 up to and including the year 200, etc. Given a year, return the century it is in.

```java
public class Solution {
  public static int century(int number) {
    // Your solution
  }
}
```

<details><summary>Solution</summary>

```java
public class Solution {
  public static int century(int number) {
    return (int)(Math.ceil(number / 100.0)); 
  }
}
```

</details>

---

**[⬆ Back to Top](#challenges)**

## Even or Odd

Create a function that takes an integer as an argument and returns "Even" for even numbers or "Odd" for odd numbers.

```java
public class EvenOrOdd {
  public static String even_or_odd(int number) {
    // Your solution
  }
}
```

<details><summary>Solution</summary>

```java
public class EvenOrOdd {
  public static String even_or_odd(int number) {
    return number % 2 == 0 ? "Even" : "Odd";
  }
}
```

</details>

---

**[⬆ Back to Top](#challenges)**

## Find the Odd Int

Given an array of integers, find the one that appears an odd number of times. There will always be only one integer that appears an odd number of times.

```java
public class FindOdd {
  public static int findIt(int[] a) {
    // Your solution
  }
}
```

<details><summary>Solution</summary>

```java
import static java.util.Arrays.stream;

public class FindOdd {
  public static int findIt(int[] arr) {
    return stream(arr).reduce(0, (a, b) -> a ^ b);
  }
}
```

</details>

---

**[⬆ Back to Top](#challenges)**

## Is n Divisible by x and y?

Create a function that checks if a number `n` is divisible by two numbers `x` AND `y`. All inputs are positive, non-zero digits.

```java
public class DivisibleNb {
  public static boolean isDivisible(long n, long x, long y) {
    // Your solution
  }
}
```

<details><summary>Solution</summary>

```java
public class DivisibleNb {
  public static boolean isDivisible(long n, long x, long y) {
    return (n % x == 0) && (n % y == 0);
  }
}
```

</details>

---

**[⬆ Back to Top](#challenges)**

## Keep Hydrated!

Nathan loves cycling. Because Nathan knows it is important to stay hydrated, he drinks 0.5 litres of water per hour of cycling. You get given the time in hours and you need to return the number of litres Nathan will drink, rounded to the smallest value.

```java
public class KeepHydrated {
  public int Liters(double time) {
    // Your solution
  }
}
```

<details><summary>Solution</summary>

```java
public class KeepHydrated {
  public int Liters(double time) {
    return (int)(time / 2);
  }
}
```

</details>

---

**[⬆ Back to Top](#challenges)**

## Multiples of 3 or 5

If we list all the natural numbers below 10 that are multiples of 3 or 5, we get 3, 5, 6 and 9. The sum of these multiples is 23. Finish the solution so that it returns the sum of all the multiples of 3 or 5 below the number passed in.

Note: If the number is a multiple of both 3 and 5, only count it once. Also, if a number is negative, return 0.

```java
public class Solution {
  public int solution(int number) {
    // Your solution
  }
}
```

<details><summary>Solution</summary>

```java
public class Solution {
  public int solution(int number) {
    int sum = 0;
    for (int i = 3; i < number; i++) {
      if (i % 3 == 0 || i % 5 == 0) {
        sum += i;
      }
    }
    return sum;
  }
}
```

</details>

---

**[⬆ Back to Top](#challenges)**

## Multiply

This code does not execute properly. Try to figure out why.

```java
public class Multiply {
  public static Double multiply(Double a, Double b) {
    return a * b
  }
}
```

<details><summary>Solution</summary>

```java
public class Multiply {
  public static Double multiply(Double a, Double b) {
    return a * b;
  }
}
```

</details>

---

**[⬆ Back to Top](#challenges)**

## Vowel Count

Return the number (count) of vowels (a, e, i, o, u) in the given string. The input string will only consist of lower case letters and/or spaces.

```java
public class Vowels {
  public static int getCount(String str) {
    // Your solution
  }
}
```

<details><summary>Solution</summary>

```java
public class Vowels {
  public static int getCount(String str) {
    int vowelsCount = 0;
    String vowels = "aeiou";
    for (int i = 0; i < str.length(); i++) {
      if (vowels.contains(String.valueOf(str.charAt(i)))) {
        vowelsCount++;
      }
    }
    return vowelsCount;
  }
}
```

</details>

---

**[⬆ Back to Top](#challenges)**
