Stack Implementation Using LifoQueue (Max Size 5) 🔄
This Python program demonstrates a stack implemented using the LifoQueue class from the queue module. It allows up to 5 elements, checks if the stack is full, and then prints the elements in reverse (LIFO) order.

🎯 Aim
To create a Python program that:

Implements a stack using LifoQueue with a maximum size of 5
Adds user-inputted values to the stack
Checks whether the stack is full
Prints the stack elements in reverse order (LIFO)
📋 Algorithm
Import the LifoQueue class from the queue module.
Create a stack with a maximum size of 5.
Read the number of elements (n) to be added to the stack.
Loop n times:
Read a value from the user.
Use put() to push it onto the stack if it's not full.
Use full() to check if the stack is full and print the result.
Use get() repeatedly to pop and print elements in reverse order.
Program
from queue import LifoQueue

stack = LifoQueue(maxsize=5)

n= int(input())

for i in range(n):

stack.put(input())
print(stack.full())

for i in range(n):

print(stack.get())
🧪 Sample Input and Output
image
Result:
The program is excuted and verified.
