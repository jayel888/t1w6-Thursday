## Control Flow
Order in which lines of code are executed in a program.

print("Hello, welcome to programming with Python")

a = 10
b = 5
result = a + b

print(f"The result of adding {a} and {b} is {result}")

print("Thank you")

# Sequential control flow
Execution of code statements one after another, in the order they appear in the program

# Conditional control flow / Control Flow
Execution of code statements based on some input

if tomorrow is Saturday
    set alarm for 7
if tomorrow if Tueday
    set alarm for 6

# Boolean Data Type Re-visit
Data type that has two values: True and False. Boolean values are used to control the flow of the program.

# Comparison Operators / Relational Operators
Decide the relationship between the operands. Result of the comparison is a boolean value (True/False)

if tomorrow == Saturday: 
    set alarm for 7
if tomorrow == Tuesday
    set alarm for 6

# if, elif, else
Simplest form of AI. (you could say that)
'if' checks the condition, if true, the intended blocks get executed, if false, it skips the intended blocks

today = "Tuesday"

if today == "Monday":
    print("Set an alarm for 5AM")
elif today == "Tuesday":
    print("Set an alarm for 6AM")
elif today == "Saturday":
    print("Set an alarm for 7AM")

temperature = 40

if temperature > 35:
    print("It's hot outside.")
elif temperature < 15:
    print("It's cold outside.")
else:
    print("The weather is mild.")


# pass
Does nothing, just passes for now. Syntax error if line is commented out.

# Boolean Operators
AND, OR, NOT. Operands needs to be boolean as well.

age = 20
has_permission = False

if age >= 18:
    if has_permission:
        print("Access Granted.")
    else:
        print("Access Denied.")
else:
    print("Access Denied")

if age >= 18 and has_permission:
    print("Access Granted.")
else:
    print("Access denied.")

# Ternary Operator
Condense series of code to one line, where applicable

print("Access Granted.") if age >= 18 and has_permission else print("Access denied.")

temperature = 30

if temperature > 30:
    message = "it's hot outside"
else:
    message = "it's not hot outside"

print (message)

message = "It's hot outside" if temperature > 30 else "it's not hot outside"

print(message)

# Match-case / Switch-case
Control flow, similar to switch statement in other programming languages

day_number = 3

match day_number:
    case 1:
        day_name = "Monday"
    case 2:
        day_name = "Tuesday"
    case 3:
        day_name = "Wednesday"
    case 4:
        day_name = "Thursday"

print(day_name)

# Activity
Write a python scipt that asks the user to input a numerical score and categorises it into grades (A, B, C, D, E, F) based on the following criteria
90-100: A
80-89: B
70-79: C
60-69: D
<60 = F

#Prompt the user to enter a score
score = int(input("Enter the Score (0-100): "))

# Determines the grade based on the score
if score >= 90 and score <= 100:
    grade = "A"
elif score >= 80:
    grade = "B"
elif score >= 70:
    grade = "C"
elif score >= 60:
    grade = "D"
else:
    grade = "F"

print (f"The grade for {score} is {grade}")