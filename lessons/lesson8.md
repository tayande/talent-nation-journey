## LESSON 8.1: TYPE CASTING
### Type Casting
Changing a value from one data type to another.
### int()
A built-in function that converts text characters or decimals into a whole integer.
### float()
A built-in function that converts text characters or whole integers into a decimal value.
### str()
A built-in function that converts numbers or boolean values into text characters.
### Conversion Error
An execution error that occurs when you try to convert a value into a format that does not make sense.
### Step 1: Why We Need Type Casting
In programming, data types behave differently. Numbers can perform math operations, while text strings can only be joined together (concatenated). Sometimes your script receives data as text (like when a customer types an order on a touchscreen), but you must perform math calculations on it before making the smoothie.
### Step 2: Converting Text to Numbers: int() and float()
To convert a text string containing digits into a number, we use int() for whole counts and float() for quantities with decimal points.
- int() converts text to a whole number: "2" becomes 2.
- float() converts text to a decimal number: "1.5" becomes 1.5.
### Step 3: Converting Numbers to Text: str()
To print a number on the paper label or combine it with a text message, you must convert the numeric value back into a string of text characters using str().
### Step 4: Handling Conversion Errors
If the user inputs characters that do not represent numbers, trying to convert them will crash the program. We must verify that the characters are valid digits before we attempt to convert them. For instance:
```python
user_input = "banana"

# Check if the string consists entirely of digits (0-9)
if user_input.isdigit():
    banana_count = int(user_input)
    print("Conversion successful!")
else:
    print("Warning: That is not a valid number! Defaulting to 0.")
    banana_count = 0
```
