## LESSON 4.1: HOW PYTHON RUNS YOUR CODE (WITH OUTPUT REDIRECTION AND EXIT CODES)
This is the lesson that teaches how the python code that is written in a file gets interpreted or translated into what the coputer can actually understand and work with. There is a translator that converts the python code into machine code and it has two types:
- compiler: This reads all the source code into memory, builds an executable version of the code before running it
- Enterpreter: This reads the code line by line from top to bottom and then executes as it reads.
Python uses the Enterpreter to run and executes it's code.
### Step 1: Interpreter vs. Compiler
### Step 2: Execution Order — Top to Bottom
### Step 3: The print() Function
### Step 4: Redirecting Output with >
Normally, when you run a Python script, the output prints directly inside your terminal window:
```python
$ python cake.py
Starting the kitchen machine...
Grinding espresso beans...
```
If you want to save this output directly onto a new index card (file) inside your folder instead of displaying it on the screen, you can use the redirection operator > in your terminal:
`$ python cake.py > daily_log.txt`

You can view the saved file contents in your terminal using the cat command:
```python
$ cat daily_log.txt
Starting the kitchen machine...
Grinding espresso beans...
```
### Step 5: Exit Status — Success or Failure?
Every time a program finishes executing, it returns a integer value to the operating system called an Exit Status (or exit code):

An exit status of 0 indicates success—everything executed as expected without errors.
Any non-zero exit status (such as 1, 2, or 127) indicates a failure or runtime error.
You can query the exit status of the last executed command in your terminal using the special shell variable $?:
`echo $?`
### Step 6: Command Chaining with && and ||
You can run multiple terminal commands sequentially on a single line, controlling whether the subsequent commands run based on the success or failure of the first.

1. The AND Operator (&&)
Runs the second command only if the first command succeeded (returned an exit status of 0).
`python3 safe_recipe.py && echo "Action approved!"`
Because safe_recipe.py succeeds, "Action approved!" will be printed to the screen.
2. The OR Operator (||)
Runs the second command only if the first command failed (returned a non-zero exit status).
`python3 broken_recipe.py || echo "Warning: Action failed!"`
Because broken_recipe.py crashes, the terminal executes the fallback command and prints the warning message.
3. Combining Both Operators
You can combine both operators to handle success and failure paths on a single execution line:
`python3 cake.py > receipt.txt && echo "Receipt printed!" || echo "Fulfillment failed!"`
 