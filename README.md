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
