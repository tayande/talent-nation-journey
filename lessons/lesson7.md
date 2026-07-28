## LESSON 7.1: OPERATORS AND EXPRESSIONS
### Arithmetic Operators
These are math tools used to perform basic calculations: 
- (add) +
- (subtract) - 
- (multiply) * 
- (divide) / 
- (exponent) **
### Comparison Operators
These are tools used to compare values against each other, outputting a True or False result.
### Logical Operators
These are operators used to join multiple boolean conditions together: and, or, not.
### Expression
A combination of values, variables, and operators that resolves down to a single value. for example, checking if `milk_ounces >= 8`
### Operator Precedence
This is seen as the strict order of execution that dictates which operations are evaluated before others.
### Step 1: Arithmetic Operators (Math Tools)
Arithmetic operators let the robot perform calculations on our kitchen assets:
```python
+ Addition: 2 + 3 evaluates to 5
- Subtraction: 5 - 2 evaluates to 3
* Multiplication: 2 * 3 evaluates to 6
/ Division: 6 / 2 evaluates to 3.0 (always outputs a decimal float)
** Exponent (Power): 2 ** 3 evaluates to 8 ($2^3$)
```
### Step 2: Comparison Operators (Checking Conditions)
Comparison operators allow the robot to evaluate states and return a simple True or False boolean value:
```python
== Equals: 5 == 5 is True, 5 == 3 is False
!= Not Equal: 5 != 3 is True, 5 != 5 is False
> Greater Than: 5 > 3 is True
< Less Than: 3 < 5 is True
>= Greater Than or Equal To: 5 >= 5 is True
<= Less Than or Equal To: 3 <= 5 is True
```
### Step 3: Logical Operators (Combining Conditions)
Logical operators let us combine multiple boolean statements into a single decision:
```python
and: Evaluates to True only if both sides are True.
or: Evaluates to True if at least one side is True.
not: Inverts the boolean value (turns True to False, or False to True).
```
### Step 4: Operator Precedence (Order of Evaluation)
When you combine multiple math and logic operators on a single line, Python evaluates them in a strict order (from highest priority to lowest):
```python
** (Exponentiation)
*, / (Multiplication, Division)
+, - (Addition, Subtraction)
==, !=, >, <, >=, <= (Comparisons)
not (Logical NOT)
and (Logical AND)
or (Logical OR)
```