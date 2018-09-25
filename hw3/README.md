# CS101A Assignment 3

> 11510225 Yuxing Hu (胡与兴)

### Question 1

```
add 2 
bne 9 1
```

This program will continue to run forever. 

As the initial value is set to 0, first line will add 2 to it, and second will evaluate whether the answer is equal to 9, which is impossible because after first line the value of r is always be odd. So it become an infinitely loop.

### Question 2

```
add 126
blt 126 1
add 2 
bgt 127 1
```

The starting value of register should be 0, next instruction should be line 1.

| Steps     | Value of register | Next instruction |
| --------- | ----------------- | ---------------- |
| add 126   | 126               | 2                |
| blt 126 1 | 126               | 3                |
| add 2     | 128               | 4                |
| bgt 127 1 | 128               | 1                |
| add 126   | 254               | 2                |
| blt 126 1 | 254               | 3                |
| add 2     | 0                 | 4                |
| bgt 127 1 | 0                 | 5                |

 The instructions will stop after the value equals to 0, at 8th step.

### Question 3

```
add 126
add 1
bgt 127 1 
blt 252 2
```

The starting value of register should be 0, next instruction should be 1.

| Steps     | Value of register | Next instruction |
| --------- | ----------------- | ---------------- |
| add 126   | 126               | 2                |
| add 1     | 127               | 3                |
| bgt 127 1 | 127               | 4                |
| blt 252 2 | 127               | 2                |
| add 1     | 128               | 3                |
| bgt 127 1 | 128               | 1                |
| add 126   | 254               | 2                |
| add 1     | 255               | 3                |
| bgt 127 1 | 255               | 1                |
| add 126   | 125               | 2                |
| add 1     | 126               | 3                |
| bgt 127 1 | 126               | 4                |
| blt 252 2 | 126               | 2                |
| add 1     | 127               | 3                |

 So there's a loop go through line 2 -> 3 -> 4 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 ->3 -> 4 -> 2 -> 3 -> 2.