# 2. Recursion and Backtracking
## 2.2 What is Recursion?
- Function which call itself
- It is importang to ensure that the recursion is terminate
## 2.3 Why Recursion?
- Shorter and easier to write
- Example uses:
    - Sort
    - Search
    - and Traversal problems
## 2.4 Format of a Recursion Function
Recursive function contains:
- a task by calling itself to perform the subtasks
- a subtask that it can perform without calling itself (base case)
    - terminate the function
```
if (test for the base case)
  return (some base case value)
else if(test for another base case)
  return (some other base case value)
else
  return (some work and then a recursive call)
```

