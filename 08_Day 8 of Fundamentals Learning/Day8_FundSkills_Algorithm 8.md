# ALGORITHMS 8

### 1. How can we compare between two algorithms written for the same problem?
The complexity of an algorithm is a technique that is used to categorise how efficient it is in comparison to other algorithms. It focuses on how the size of the data set to be processed affects execution time. In computing, the algorithm's computational complexity is critical. It is a good idea to categorise algorithms according to how much time or space they take up and to describe how much time or space they take up as a function of input size.

#### Complexity of Time: 
    - The running time of a program as a function of the size of the input is known as time complexity.
#### Complexity of Space:
    - Space complexity examines algorithms based on how much space they require to fulfil their tasks. In the early days of computers, space complexity analysis was crucial (when storage space on the computer was limited).

Note: Nowadays, a lack of space is rarely an issue because computer storage is plentiful. Therefore, it is mostly the Time Complexity that is given more importance while evaluating an Algorithm.

### 2. What do you understand by the best case, worst case and average case scenario of an algorithm?
The mathematical foundation/framing of an algorithm's run time performance is defined by asymptotic analysis. We can easily determine the best case, average case, and worst-case scenarios of an algorithm using asymptotic analysis.

#### Best Case Scenario of an Algorithm:
    - The best-case scenario for an algorithm is defined as the data arrangement in which the algorithm performs the best. Take a binary search, for example, where the best-case scenario is if the target value is in the very centre of the data we are looking for. The best-case scenario for binary search would have a time complexity of O(1) or constant time complexity.

#### Worst Case Scenario of an Algorithm:
    - The worst collection of input for a given algorithm is referred to as the worst-case scenario of an Algorithm. For example, quicksort can perform poorly if the pivot value is set to the largest or smallest element of a sublist. Quicksort will degenerate into an algorithm with a time complexity of O(n^2), where n is the size of the list to be sorted.

#### Average Case Scenario of an Algorithm:
    - The average-case complexity of an algorithm is the amount of some computational resource (usually time) used by the process, averaged over all possible inputs, according to computational complexity theory. For example, the average-case complexity of the randomised quicksort algorithm is O(n*log(n)), where n is the size of the list to be sorted.