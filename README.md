# Python.notes
This is Python Note




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



### First Example: CalculateAutomobile

```python
# Find How many two-wheeler and four-wheeler are made

# 130 + 70 = 200 vehicles
# (70 * 4) + (130 * 2) = 540 wheels

def CalculateAutomobile(total, wheels):
    if int(wheels) > int(total):
        two_wheeler = ((4 * int(total)) - int(wheels)) // 2
        two_wheeler = int(two_wheeler)
        if two_wheeler > 0:
            four_wheeler = int(total) - two_wheeler
            print("By providing info " + str(two_wheeler) + " Two-wheeler are made and " + str(four_wheeler) + " four-wheeler are made ")
        else:
            print("Sorry, your data is not valid for this")
    else:
        print("Sorry, your data is invalid for this")

CalculateAutomobile(200, 600)
```

### Second Example: MakeDecision

```python
# ###*** for this makeList = list(userInput)

def MakeDecision(userInput):
    s = userInput
    countOfStar = 0
    countOfHash = 0
    
    for item in s:
        if item == "#":
            countOfHash += 1
        else:
            countOfStar += 1
            
    print(countOfStar - countOfHash)
    
    if countOfHash > countOfStar: 
        print("Negative Integer")
    elif countOfHash < countOfStar:
        print("Positive Integer")
    elif countOfHash == countOfStar:
        print("Equal")
    else:
        print("Invalid Input")

MakeDecision("###***")
```

### Third Example: CountOfPrior

```python
# [-2, -5, -1, -8, -3] and [5, 2, 8, 4, 9, 1] for both use float(-inf) comparing the previous greater element

listOfElement = [-2, -5, -1, -8, -3]

def CountOfPrior(listOfElement):
    count = 0 
    max_value = float('-inf')
    
    for element in listOfElement:
        if element > max_value:
            print(element, max_value)
            count += 1
            max_value = element 
        
    return count 

result = CountOfPrior(listOfElement) 
print(result)
```


