## LESSON 5.1: PYTHON KEYWORDS AND SYNTAX
There are certain things all languages have:
- vocabulary: Which are words you can use
- grammer: Which are the rules involved in putting the words together
Python as a programming language just like the others has the following as well:
- keywords: Special words that have meaning in python
- syntax: The rules for writing python code correctly.
### Step 1: What Are Python Keywords?
They are special words that python already uses for specific purposes. You can't use them as variable names, function names, or anything else.
#### How to check if a work is a keyword:
```python
import keyword

# Check if a word is a keyword
print(keyword.iskeyword("if"))      # True
print(keyword.iskeyword("hello"))   # False
print(keyword.iskeyword("for"))     # True
print(keyword.iskeyword("my_var"))  # False

```
### Step 2: Syntax Rules — The Grammar of Python
#### Rule 1: Colons (:)
```python
# ✅ Correct — colon after if statement
if x > 5:
    print("x is greater than 5")

# ❌ Wrong — missing colon
if x > 5
    print("x is greater than 5")  # ERROR! Missing colon
```
#### Rule 2: Indentation (Spaces at the start)
Python uses this to show what belongs to a block of code and what does not. All lines of code on the same block or in the same block must have the same amount of indentation.
```python
# ✅ Correct — all lines indented the same amount
if x > 5:
    print("x is greater than 5")
    print("That's a big number!")

# ❌ Wrong — inconsistent indentation
if x > 5:
    print("x is greater than 5")
      print("That's a big number!")  # ERROR! Indentation mismatch

```
#### Rule 3: Quotes must match
for instance:
```python
# ✅ Correct — both quotes are the same
print("Hello")   # Double quotes
print('Hello')   # Single quotes

# ❌ Wrong — quotes don't match
print("Hello')   # ERROR! Mixed quotes

```
#### Rule 4: Parentheses must close
for instance:
```python
# ✅ Correct — parentheses match
print("Hello")

# ❌ Wrong — missing closing parenthesis
print("Hello"   # ERROR! Missing parenthesis
```
#### Keywords must be spelled correctly
for instance:
```python
# ✅ Correct
if x > 5:
    print("Hello")

# ❌ Wrong — misspelled keyword
if x > 5:       # "if" is correct
    print("Hello")

# ❌ Wrong — another misspelling
if x > 5:       # "if" is correct, but...
    prnt("Hello")  # ERROR! "prnt" is not a keyword or function
```
### Step 3: Common Syntax Errors and How to Fix Them
#### Error 1: Missing colon
for instance:
```python
# ❌ Wrong
age = 25
if age > 18
    print("You are an adult")
```
#### Error 2: Wrong indentation
Understood 
#### Error 3: Misspelled keyword
Understood
#### Error 4: Missing quote
Understood
#### Error 5: Mixed quotes
Understood
### Step 4: Comments — Notes for Humans
Comments are notes in a python code, go code, etc that the translator ignores completely. they're used for human cosumption. In python, a line of comment starts with a `#`
#### Why use comments?
- Explain what your code does — so you remember later
- Explain why you did something — so others understand
- Leave notes for yourself — "TODO: fix this later"
- Temporarily disable code — testing without deleting
Comments should explain why you're doing something, not what you're doing. The code already shows what you're doing.
### Step 5: Putting It All Together
Let's look at a complete script with keywords, syntax, and comments:
```python
# Example script — calculates the cost of coffee orders

# Set prices for different drinks
espresso_price = 3.50
latte_price = 4.50
cappuccino_price = 4.00

# Get the number of drinks ordered
num_espresso = 2
num_latte = 3
num_cappuccino = 1

# Calculate the total cost
total = (num_espresso * espresso_price) + \
        (num_latte * latte_price) + \
        (num_cappuccino * cappuccino_price)

# Check if total is above the minimum for a discount
discount = 0.10
if total > 20:
    total = total - (total * discount)  # Apply 10% discount
    print("Discount applied!")
else:
    print("No discount available")

# Print the final total
print(f"Total cost: ₦{total}")
print("Thank you for your order!")
```