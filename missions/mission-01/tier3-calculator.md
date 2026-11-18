# The calculator task
## The core part
### For Addition
- Input: 20, 5
- Processing: addition (20 + 5)
- Output: 25

### For subtraction
- Input: 20, 5
- Processing: subtraction (20 − 5)
- Output: 15

### For Multiplication
- Input: 20, 5
- Processing: Multiplication (20 * 5)
- Output: 100

### For division
- Input: 20, 5
- Processing: division (20 / 5)
- Output: 4

## The reasoning challenge
#### first question: what happens when the program attempts 20 / 0? is there any valid answer?
No, there is no valid answer for this, if this operation is attempted in python, there would be a ZeroDivisionError since 20 cannot be divided by 0.
#### second question: what should a well-designed program do when an input makes the operation impossible?
A well designed program that is performing a division should first of all check and verify if the second input or number is not zero, if it is then the program should tell the user that division cannot be performed on 0 and END the program. But if the second number the user enters for the operation is not 0, then the program should go ahead and perform the operation and return the result to the user. This guard is necessary so that the program would not crash on attempting the operation.  Below is a practical example of how such a program would work.

### For division by zero. Now the input is 20 and 0
- Input: a, b
- check the second input
- if the second input is 0, return a "cannot divide by zero" error message and END
- if not, processing: division (a / b)
- return the result for the operation to the user and END
