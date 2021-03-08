![java](images/java-logo.png)

# [Codewars](https://www.codewars.com/) Java Solutions

## Challenges

|  Kyu  | Questions                                   | Easy  | Medium | Hard  |
| :---: | :------------------------------------------ | :---: | :----: | :---: |
|   6   | [Multiples of 3 or 5](#multiples-of-3-or-5) |   ⭐   |        |       |
|   8   | [Multiply](#multiply)                       |   ⭐   |        |       |

---

## Multiples of 3 or 5

If we list all the natural numbers below 10 that are multiples of 3 or 5, we get 3, 5, 6 and 9. The sum of these multiples is 23. Finish the solution so that it returns the sum of all the multiples of 3 or 5 below the number passed in.

Note: If the number is a multiple of both 3 and 5, only count it once. Also, if a number is negative, return 0.

```java
public class Solution {

  public int solution(int number) {
    // Your solution here
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
