# code_fun

Python Practice Challenges
Here are a dozen bite-sized, hands-on challenges—organized by topic—to get you coding immediately. Pick one from each section, solve it in a single .py file (or Jupyter cell), and move on. No tutorials—just code!

# 1. Data Types & Syntax
Swap Without a Temp
Write a snippet that swaps the values of a and b without using a third variable.

python
Copy
Edit
a = 5
b = 12

print(a, b)  # should print: 12 5
# vowel Counter
Given a string, count how many vowels (a, e, i, o, u) it contains. Return a dictionary mapping each vowel to its count.

# Flatten Nested List
Write a one-line list comprehension that flattens [[1,2],[3,4],[5]] into [1,2,3,4,5].

# Word Frequency
Read a sentence from the user, split into words, and build a dict of word→count. Use .split() and iterate.

# Unique Preserver
Given a list with duplicates, produce a tuple of its unique items in their original order (hint: use a set to track seen).

# #  2. Control Flow
FizzBuzz Variant
For numbers 1–50, print “Fizz” if divisible by 3, “Buzz” if by 5, “FizzBuzz” if by both—and the number otherwise.

#  Prime Sieve
Using a for loop and if checks, generate a list of all primes ≤ 100.

# Guessing Game
Build a CLI loop that picks a random number 1–20 (use random.randint), lets the user guess, and tells them “higher”/“lower” until they get it right.

# Multiplication Table
Print an n×n table (aligned columns) for n read from the user.

# List Comprehensions
Using one comprehension, build a list of squares of odd numbers from 1–20.

# # 3. Functions & Modules
# Reusable Factorial
Write def factorial(n): that returns n!, and include a docstring. Test it on a few values.

# Perfect Squares
In a new module math_utils.py, implement is_perfect_square(n) using math.sqrt. Then in main.py, import and test it.

# CSV Reader
Use the built-in csv module to read a small CSV (you can make up data), compute the average of a numeric column, and print it.

# JSON API Call
In fetch.py, import json and urllib.request (or requests if installed) to GET https://api.github.com and pretty-print the JSON.

# Module Structure
Organize two modules—data.py with a function that returns a list, and plot.py that imports it and prints or plots (matplotlib) those values.

# 4. Error Handling
Safe Division
Write def safe_div(a, b): that returns a/b but catches ZeroDivisionError and prints “Cannot divide by zero.” Return None in that case.

# User Input Validator
Loop asking the user for an integer until they actually enter one—use try/except ValueError around int(input(...)).

# File Reader with finally
Open a file path from the user, read its contents, print the first line, and ensure the file is closed via a finally block.

# Assert Positive
In your factorial(n) from above, add assert n >= 0, "n must be non-negative" and see it trigger for n=-1.

# Chained Exceptions
Inside a try, raise a custom exception if a condition fails, catch it, and re-raise it with additional context.

# 5. Virtual Environments
Create & Activate

venv:

bash
Copy
Edit
python3 -m venv ds_venv
source ds_venv/bin/activate      # macOS/Linux
ds_venv\Scripts\activate.bat     # Windows
conda:

bash
Copy
Edit
conda create -n ds_env python=3.10
conda activate ds_env
Install & Import
Inside your new venv, pip install requests pandas (or any small package). Write a short script that imports them and prints their versions:

python
Copy
Edit
import requests, pandas as pd
print(requests.__version__, pd.__version__)
Freeze & Reproduce
Run pip freeze > requirements.txt. In a fresh venv, pip install -r requirements.txt and verify imports still work.

# Isolated CLI Tool
Package one of your small scripts (e.g. the JSON fetcher) as an entry-point in setup.py or use pipx to install it locally and run it from the command line anywhere.

📈 Integrated Mini-Challenge
Combine everything in a single script:

Fetch live weather (use requests on OpenWeatherMap’s free API; you’ll need to sign up for an API key).

Parse the JSON into Python types, handle missing fields with try/except.

Summarize the forecast (e.g. average temp, max/min).

Use a comprehension to list dates where rain is expected.

Wrap logic in functions in a module you import.

Run it inside a new venv and freeze your requirements.

