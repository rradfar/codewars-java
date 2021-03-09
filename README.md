![java](images/java-logo.png)

# [Codewars](https://www.codewars.com/) Java Solutions

## Challenges

|  Kyu  | Questions                                   |
| :---: | :------------------------------------------ |
|   8   | [Even or Odd](#even-or-odd)                 |
|   6   | [Multiples of 3 or 5](#multiples-of-3-or-5) |
|   8   | [Multiply](#multiply)                       |
|   7   | [Vowel Count](#vowel-count)                 |

---

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
