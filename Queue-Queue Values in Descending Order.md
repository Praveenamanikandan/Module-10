# Queue-Queue Values in Descending Order Using Python 

This Python program simulates a queue using a list, removes the first two elements (FIFO order), and displays the remaining values in descending order.

##  Aim

To write a Python program to:
- Accept user inputs into a list (queue)
- Remove the first two elements (simulating dequeue)
- Display the remaining values in **descending order**

##  Algorithm

1. Create an empty list `q`.
2. Read an integer `n` to determine how many elements will be added.
3. Loop `n` times:
   - Read an input value.
   - Append it to the list `q`.
4. Remove the first element using `pop(0)`.
5. Remove the second element using `pop(0)` again.
6. Sort the list in descending order.
7. Print the updated list.

##  Program: 
```
from collections import deque

# Read number of elements
n = int(input())

# Initialize deque
dq = deque()

# Read n string values
for _ in range(n):
    dq.append(input())

# Remove the first two elements from the front
for _ in range(min(2, len(dq))):
    dq.popleft()

# Print the resulting deque
print(dq)

```
### Output:
<img width="1107" height="412" alt="image" src="https://github.com/user-attachments/assets/f76ad8de-f7b0-4363-b92e-161548b1be21" />

## Result:
The Program was executed successfully
