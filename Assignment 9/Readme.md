# CS101A Assignment 9

> 11510225 Yuxing Hu (胡与兴)

#### 1: Program in the machine language 

a. Move the value at memory location D8 to memory location B3

| Address | Contents |
| ------- | -------- |
| 00      | 10       |
| 01      | D8       |
| 02      | 30       |
| 03      | B3       |
| 04      | C0       |
| 05      | 00       |

b. Interchange the values stored at memory locations D8 and B3.

| Address | Contents |
| ------- | -------- |
| 00      | 10       |
| 01      | D8       |
| 02      | 11       |
| 03      | B3       |
| 04      | 30       |
| 05      | B3       |
| 06      | 31       |
| 07      | D8       |
| 08      | C0       |
| 09      | 00       |

c. If the value stored in memory location 44 is 00, then place the value 01 in memory location 46; otherwise, put the value FF in memory location 46. 

| Address | Contents |
| ------- | -------- |
| 00      | 11       |
| 01      | 44       |
| 02      | 20       |
| 03      | 00       |
| 04      | 22       |
| 05      | 01       |
| 06      | B1       |
| 07      | 0A       |
| 08      | 22       |
| 09      | FF       |
| 0A      | 32       |
| 0B      | 46       |
| 0C      | C0       |
| 0D      | 00       |

#### 2: Perform the indicated operations

a. 11111111

b. 11100000

#### 3: 1-bit left circular shift

a. AB = (1010 1011) -> (0101 0111) = 57

b. 5C = (0101 1100) -> (1011 1000) = B8

c. B7 = (1011 0111) -> (0110 1111) = 6F

d. 35 = (0011 0101) -> (0110 1010) = 6A

#### 4. Write a program

11E0 (LOAD register 1 with the contents of memory cell E0.) 

A102 (ROTATE the contents of register 1 to the left by 2 bits.) 

220F (LOAD register 2 with the value 0F.)

8021 (AND registers 2 and 1, leaving the result in register 0.) 

30E1 (STORE the contents of register 0 in memory cell E1.) 

C000 (HALT.)