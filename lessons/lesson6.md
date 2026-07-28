## LESSON 6.1: VARIABLES AND PRIMITIVE TYPES
In programming, variables work like a labelled storage jar with a certain content. The computer memory is a large digital countertop, if you do not store your stuff in a labelled container, you would not know how to access them when you need them, and you would definitely loose track of them. *** A variable *** is a labeled container in the computer's memory used to store a specific piece of information.
### Step 1: Creating Variables and Assignment
To create a variable in Python, you write the container's label on the left, use the assignment operator (=), and put the contents on the right. 
### Step 2: The Four Primitive Types
Python has a way of grouping everything we store to avoid mix up. for instance, when you store a name in a variable, python has to know what kind of content is in that variable. There are four basic types of data we store in our jars:
```python
# 1. Integer (int) - Whole, countable items
bean_count = 15

# 2. Float (float) - Measurable decimals/fractions
water_cups = 1.5

# 3. String (str) - Plain text characters wrapped in quotes
roast_level = "Medium Dark"

# 4. Boolean (bool) - Simple True or False state
is_caffeinated = True
```
### Step 3: Checking Types with type()
If you ever lose track of what type of ingredient is inside a jar, you can use Python's built-in type() function to scan the container.

