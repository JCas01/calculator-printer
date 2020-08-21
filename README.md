# Calculator Printer

You probably own a pocket calculator. Have you ever looked closely at its screen? Most calculator screens use a seven-segment display, so named because there are 7 "bars" that can be switched on and off. The digit 8 is the most illustrative, as it has all the bars switched on. In contrast, the digit 1 only has the two right-most bars on, and all the others are off.

Write a program that reads two integers - a number and a width - and prints the number out as it would appear on a seven-segment display with that width. You can assume that the number will always be non-negative and that the width will be positive.

Use a dash ("-") for horizontal segments, and a pipe ("|") for vertical segments. Each digit in a multiple-digit number should be separated by a space, and every digit has precisely the same dimensions (padded with spaces as necessary):

```width + 2``` characters wide (left- and rightmost bars)
```2*width + 3``` characters tall (top, middle, and bottom bars)
Here is an example with each digit and a width of 1 (note the highlighted spaces at the end of the line):
```
Number: 1234567890
Width: 1
     -   -       -   -   -   -   -   - 
  |   |   | | | |   |     | | | | | | |
     -   -   -   -   -       -   -     
  | |     |   |   | | |   | | |   | | |
     -   -       -   -       -   -   - 
```
Notice how each digit is the same size, with different bars switched on as appropriate. Each line is exactly the same length, padded with spaces as necessary. Here is an example with a width of 2:

```
Number: 912768
Width: 2
 --        --   --   --   -- 
|  |    |    |    | |    |  |
|  |    |    |    | |    |  |
 --        --        --   -- 
   |    | |       | |  | |  |
   |    | |       | |  | |  |
 --        --        --   -- 
```

And finally, an example with a width of 3:

```
Number: 8453
Width: 3
 ---         ---   --- 
|   | |   | |         |
|   | |   | |         |
|   | |   | |         |
 ---   ---   ---   --- 
|   |     |     |     |
|   |     |     |     |
|   |     |     |     |
 ---         ---   --- 
```
