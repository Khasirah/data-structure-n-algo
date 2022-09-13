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
example:
```
// calculates factorial of a positive integer
int Fact(int n) {
    if (n == 1) {
        return 1;
      }
    if (n == 0) {
        return 1;
      }
    else {
        return n * Fact(n-1);
      }
  }
```
## 2.5 Recursion and Memory (Visualization)
- each recursive call make a new copy of that method (only the variable) in memory.
- once method end the copy is removed from memory.

let us consider our factorial function. the visualization of factorial function with n = 4 will look like:
![visualization recursion and memory](https://i0.wp.com/studyalgorithms.com/wp-content/uploads/2013/10/2.png?ssl=1)
> the box is representative of memory, so when the process at box that contain 1 and value 1 will return to box that contain 2*1!, the box with contain 1 will remove from memory and so on.

## 2.6 Recursion vs Iteration
which way is better? recursion or iteration. the answer is depends on what we are trying to do.

**Recursion**
- terminates when a base case is reached
- each recursive call requires extra space on the stack frame (memory)
- if we get infinite recursion, the program may run out of memory and result in stack overflow
- solutions to some probelms are easier to formulate recursively

**Iteration**
- Terminate when a condition is proven false
- each iteration does not require extra space
- an infinite loop could loop forever since there is no extra memory being created
- itrative solutions to a problem may not always be as obvious as a recursive solution

## 2.7 Notes on Recursion
- recursive algorithms have two types of cases, recursive case and base cases
- must terminate
- generally, iterative solution are more effecient than recursive function solutions [due to the overhead of function calls]
- any problem that can be solved recursively can also be solved iterative
- for some problem, there are no obvious iterative algorithms
- some problems are best suited for recursive solution while others are not 

## 2.8 Example Algorithms of Recursion
- fibonacci series, factorial finding
- merge sort, quick sort
- binary search
- tree traversal and many tree problems, inOrder, PreOrder, PostOrder
- graph traversal: DFS [Depth First Search] and BFS [Breadth First Search]
- dynamic programming
- divided and conquer algorithms
- towers of hanoi
- backtracking algorithms

## 2.9 What is Backtracking?
- improvement of the brute force approach
- it systematically search for a solution among all available options
- eliminate choice that are obviously not possible and proceed to recursively check only those solutions possible

## 2.10 Example Algorithms of Backtracking
- binary search: generating all binary strings
- generating k - ary string 
- N-Queens problem
- The Knapsack problem
- generalized strings
- hamiltonian cycles
- graph coloring problem
