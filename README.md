Q1 (a) – Discount Slabs:
amount = float(input("Enter the purchase amount: "))

if amount > 40000:
    discount = 0.30
elif 25000 < amount <= 40000:
    discount = 0.20
elif 10000 <= amount <= 25000:
    discount = 0.10
else:
    discount = 0

if discount > 0:
    print(f"Discount Applied: {discount*100}%")
    print(f"Final Price: {amount - (amount * discount)}")
else:
    print("No discount applicable")


  
  Q1 (b) – Print all letters except 'o' and 'e':
python
text = "Wolfeschlegelsteinhausenbergerdorff"
for char in text:
    if char not in ['o', 'e']:
        print(char, end="")


Q2 (a) – Print numbers from 1 to 10 based on index values:
python
Copy
Edit
numbers = list(range(1, 11))
# Based on index values [1,6] and [5,1]
print("Index [1:6]:", numbers[1:6])   # Output: [2, 3, 4, 5, 6]
print("Index [5:1]:", numbers[5:1])   # Output: [] because it's invalid slicing

Q2 (b) – Sum of square numbers from 10 to 20:
python
Copy
Edit
total = 0
for i in range(10, 21):
    total += i**2
print("Sum of squares from 10 to 20:", total)


Q3 (a) – File Append:
python
Copy
Edit
with open("example.txt", "a") as file:
    file.write("This line is added using file append.\n")

Q3 (b) – File Write:
python
Copy
Edit
with open("example.txt", "w") as file:
    file.write("This line is added using file write (overwrite).\n")

Q4 (a) – Class maths with two data members:
python
Copy
Edit
class Maths:
    def __init__(self, num1, num2):
        self.num1 = num1
        self.num2 = num2

  def display(self):
        print("Number 1:", self.num1)
        print("Number 2:", self.num2)

obj = Maths(10, 20)
obj.display()


@@@@@@# Define a class
class Student:
    # Attributes
    name = ""
    age = 0

# Create an object of the class
student1 = Student()

# Assign values to the object's attributes
student1.name = "Ravi"
student1.age = 20

# Print the object data
print("Student Name:", student1.name)
print("Student Age:", student1.age)

 1️⃣ Print numbers from 1 to 5
python
for i in range(1, 6):
    print(i)

✅ Example 2: Print even numbers from 2 to 10
python
for i in range(2, 11, 2):
    print(i)

✅ Example 3: Print numbers backward from 5 to 1
python
for i in range(5, 0, -1):
    print(i)

✅ Example 4: Print multiples of 3 from 3 to 15
python
for i in range(3, 16, 3):
    print(i)

✅ 1. NumPy – Numerical operations
python
import numpy as np

# Create a NumPy array and multiply each element by 2
arr = np.array([1, 2, 3])
print("NumPy Array:", arr * 2)

✅ 2. Pandas – Data analysis
python
import pandas as pd

# Create a DataFrame using a dictionary
data = {"Name": ["Amit", "Ravi"], "Age": [20, 22]}
df = pd.DataFrame(data)
print("Pandas DataFrame:\n", df)



✅ 3. Matplotlib – Plotting graphs
python
Copy
Edit
import matplotlib.pyplot as plt

# Plot a simple line graph
plt.plot([1, 2, 3], [4, 5, 1])
plt.title("Simple Plot")
plt.show()



File Handling in Python

File handling refers to the process of performing operations on a file such as creating, opening, reading,
writing and closing it, through a programming interface. It involves managing the data flow between the
program and the file system on the storage device, ensuring that data is handled safely and efficiently.
# Open the file and read its contents
with open('sanjivani.txt', 'r') as file:

File Modes in Python
When opening a file, we must specify the mode we want to which specifies what we want to do with the
file. Here’s a table of the different modes available:
Mode Description Behavior

 
