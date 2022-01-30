# Project-1
Random Password Generator

import random

uppercase_letters = "GALIHZN"
lowercase_letters = uppercase_letters.lower()
digits = "023"
symbols = "*:;="

upper, lower, nums, syms, = True, True, True, True

all = ""

if upper:
    all += uppercase_letters
if lower:
    all += lowercase_letters
if nums:
    all += digits
if syms:
    all += symbols

length = 20
amount = 10

for x in range(amount):
    password = "".join(random.sample(all, length))
    print(password)
