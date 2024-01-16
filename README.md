# Python.notes
This is Python Note


Sure, I'll format your notes and code into a more organized structure:

## Python Notes

### Variables and Data Types
```python
name = "Tony"
lName = "Stark"
age = 21
profession = "Businessman"
```

### If-Else Statement
```python
# Example if-else block
# if age > 50:
#     print("He is an adult")
# else:
#     print("He is very young")
```

### String and Methods
```python
name = "Kanhaiya Gawali"
# name.upper()
# name.lower()
# name.find('Gaw')
# name.replace("Gawali", "Yadav")
```

### Arithmetic Operators
```python
# Example of arithmetic operators
# firstDigit = input("Give first digit: ")
# secondDigit = input("Give second digit: ")
# finalResult = int(firstDigit) / int(secondDigit)
# print("Your Output is " + str(finalResult))
```

### Operator Precedence
```python
result = (3 + 5) * 5
# print(result)
```

### Comparison Operators
```python
# Comparison by > and < also == or !=
print(30 > 20)
print(30 < 20)
print(30 == 20)
print(30 != 20)
```

### If-Else Block Program
```python
userinput = input("Hello, type any number; a table is required: ")
userinput = int(userinput)
i = 1
if userinput >= 1:
    while i <= 10:
        print(i * userinput)
        i = i + 1
else:
    print("Please give a proper value")
```

### List Program
```python
import math

marks = [6.59, 7.39, 6.55, 8.18, 7.73, 9.00]
i = 0

for mark in marks:
    i = i + 1
    userResult = ((mark * 10) - 7.5)
    print("You got " + str(math.floor(userResult)) + " in Current Sem " + str(i))
```

### Break Statement in For Loop
```python
studentLife = ["Attend College", "Prepare for Exam", "Prepare for Placement", "Prepare for Growing Life also",
               "Participate in political campaign", "Destroy social harmony", "Go to Depression",
               "Make Life more complicated"]

for activity in studentLife:
    if activity == "Participate in political campaign":
        break
    print("Student perform this " + activity)
```

### Set
```python
dailyHours = {5, 6, 7, 8, 5, 6}
# print(dailyHours)
```

### Dictionary
```python
marks = {"Physics": 85, "Chemistry": 75, "Math": 80, "English": 72}
# for mark in marks:
#     print(mark)
```

### Function
```python
n1 = input("Input first number: ")
operation = input("Give which operation you perform (+, -, *, /): ")
n2 = input("Input Second number: ")


def Calculation(n1, n2, operation):
    if operation == "+":
        print(int(n1) + int(n2))
    elif operation == "-":
        print(int(n1) - int(n2))
    elif operation == "*":
        print(int(n1) * int(n2))
    elif operation == "/":
        print(int(n1) / int(n2))
    else:
        print("Please Give proper information")


Calculation(n1, n2, operation)
```

These are the organized Python notes with the code displayed in a different format.
