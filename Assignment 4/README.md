# CS101A Assignment 4

> 11510225 Yuxing Hu (胡与兴)

### Question 1: True or false

1. An algorithm with time (nlogn) is better than another with time(n2).

   **False**

2. The empty string is a proper prefix of any string whose length is larger than or equal 1.

   **True**

### Question 2: Short-answer questions

1. What is the difference in the printed output of the two routines?

   * Procedure 1:

   ```
   1
   2
   3
   4
   ```

   * Procedure 2:

   ```
   4
   3
   2
   1
   ```

2. Factorial pseudocode

   ```java
   pubilc static void factorial(int num){
       if (num == 0){
           return 1;
       } else {
           int result = num;
           num -= 1;
           while (num != 0){
               result *= num;
               num -= 1;
           }
           return result;
       }
   }
   ```

### Question 3

1. ( ( n - 1) + 1) n / 2 = n^2 / 2
2. Because this kind of algorithm has a computational complexity of O(n^2), so if we follow the rule the formula it would like: 
   * 1000 numbers: 1*(1000/100)^2 = 100 seconds
   * 10000 numbers: 1*(10000/100)^2 = 10000 seconds