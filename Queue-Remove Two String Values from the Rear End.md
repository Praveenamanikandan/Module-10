# Queue-Remove Two String Values from the Rear End in Python 

This Python program demonstrates how to manage a list of strings and remove the last two elements (i.e., from the rear of the list).

##  Aim

To write a Python program to:
- Accept `n` string values from the user
- Remove the last two values (rear end of the list)
- Display the updated list

##  Algorithm

1. Create an empty list `q`.
2. Read an integer `n` from the user (number of strings).
3. Loop `n` times:
   - Read a string input.
   - Append it to the list `q`.
4. Remove the last element using `pop()`.
5. Remove the next last element using `pop()` again.
6. Display the updated list.

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
<img width="977" height="421" alt="image" src="https://github.com/user-attachments/assets/284a7a95-fb75-4542-be6f-2b65c13208e5" />

## Result:
The Program was executed successfully

