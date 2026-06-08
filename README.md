# Queue-Queue Values in Descending Order Using Python 🧮

This Python program simulates a queue using a list, removes the first two elements (FIFO order), and displays the remaining values in descending order.

## 🎯 Aim

To write a Python program to:
- Accept user inputs into a list (queue)
- Remove the first two elements (simulating dequeue)
- Display the remaining values in **descending order**

## 🧠 Algorithm

1. Create an empty list `q`.
2. Read an integer `n` to determine how many elements will be added.
3. Loop `n` times:
   - Read an input value.
   - Append it to the list `q`.
4. Remove the first element using `pop(0)`.
5. Remove the second element using `pop(0)` again.
6. Sort the list in descending order.
7. Print the updated list.

## 🧪 Program: 
from queue import PriorityQueue

que=PriorityQueue()

n=int(input())

l=[]

for i in range(n):

    l.append(int(input()))

for number in l:

    que.put((-number, number))

while not que.empty():

    print(que.get()[1])

### Output:
<img width="430" height="625" alt="image" src="https://github.com/user-attachments/assets/a2a87615-b13c-444c-b452-1b69a14ae1b8" />

## Result:
The program is excuted and verified.

# Queue-Remove Two String Values from the Rear End in Python 🧵

This Python program demonstrates how to manage a list of strings and remove the last two elements (i.e., from the rear of the list).

## 🎯 Aim

To write a Python program to:
- Accept `n` string values from the user
- Remove the last two values (rear end of the list)
- Display the updated list

## 🧠 Algorithm

1. Create an empty list `q`.
2. Read an integer `n` from the user (number of strings).
3. Loop `n` times:
   - Read a string input.
   - Append it to the list `q`.
4. Remove the last element using `pop()`.
5. Remove the next last element using `pop()` again.
6. Display the updated list.

##  Program:
from collections import deque

q = deque()

n=int(input())

for i in range(n):

    q.append(input())

for i in range(2):

    q.popleft()

print(q)

### Output:
<img width="1241" height="448" alt="image" src="https://github.com/user-attachments/assets/8e58030a-d430-49b5-b2c5-5c7292edf087" />

## Result:
The program is excuted and verified.

# Stack Implementation Using `LifoQueue` (Max Size 5) 🔄

This Python program demonstrates a stack implemented using the `LifoQueue` class from the `queue` module. It allows up to 5 elements, checks if the stack is full, and then prints the elements in reverse (LIFO) order.

## 🎯 Aim

To create a Python program that:
- Implements a stack using `LifoQueue` with a maximum size of 5
- Adds user-inputted values to the stack
- Checks whether the stack is full
- Prints the stack elements in reverse order (LIFO)

## 📋 Algorithm

1. Import the `LifoQueue` class from the `queue` module.
2. Create a stack with a maximum size of 5.
3. Read the number of elements (`n`) to be added to the stack.
4. Loop `n` times:
   - Read a value from the user.
   - Use `put()` to push it onto the stack if it's not full.
5. Use `full()` to check if the stack is full and print the result.
6. Use `get()` repeatedly to pop and print elements in reverse order.

## Program
from queue import LifoQueue

stack = LifoQueue(maxsize=5)

n= int(input())

for i in range(n):

    stack.put(input())

print(stack.full())

for i in range(n):

    print(stack.get())

## 🧪 Sample Input and Output
<img width="443" height="523" alt="image" src="https://github.com/user-attachments/assets/edea5199-c7ee-4009-9f0b-fc9ab86d3fd5" />

## Result:
The program is excuted and verified.

# # Stack-Stack Reversal Program 🔁

This Python program demonstrates how to reverse the values in a stack using basic stack operations like push and pop.

## 🎯 Aim

To write a Python program that reverses the values in a stack using standard stack operations.

## 📋 Algorithm

1. Create an empty stack.
2. Read an integer `n` from the user (number of elements to push).
3. Loop `n` times:
   - Read an integer from the user.
   - Push it onto the stack.
4. Create an empty list called `reverse`.
5. While the stack is not empty:
   - Pop the top element.
   - Append it to `reverse`.
6. Print the reversed list.


### Program:
def insertAtBottom(s, item):
    
    if not s:
    
        s.append(item)
        
        return
    
    top = s.pop()
    
    insertAtBottom(s, item)
   
    s.append(top)

def reverseStack(s):
 
    if not s:
    
        return
 
    item = s.pop()
    
    reverseStack(s)
 
    insertAtBottom(s, item)
    
    return s

l=[]

n=int(input())

for i in range(n):

    l.append(int(input()))

print(reverseStack(l))

## 🧪 Sample Input and Output
<img width="739" height="349" alt="image" src="https://github.com/user-attachments/assets/b381b96b-6f24-4da6-916c-7edc833832df" />

## Result
The progam is excuted and verified.
