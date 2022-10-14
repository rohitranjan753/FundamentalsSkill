# ALGORITHMS 9

## Write an algorithm to swap two given numbers in Java without using a temporary variable.
    It is a trick question that is frequently asked in the interviews of various companies. This problem can be solved in a variety of ways. However, while solving the problem, we must solve it without using a temporary variable, which is an essential condition. For this problem, if we can consider the possibility of integer overflow in our solution while coming up with an approach to solving it, we can make a great impression on interviewers.

    Let us say that we have two integers a and b, with a's value equal to 5 and b's value equal to 6, and we want to swap them without needing a third variable. We will need to use Java programming constructs to solve this problem. Mathematical procedures such as addition, subtraction, multiplication, and division can be used to swap numbers. However, it is possible that it will cause an integer overflow problem. 

Let us take a look at two approaches to solve this problem:

#### Using Addition and subtraction:

    a = a + b;
    b = a - b; // this will act like (a+b) - b, and now b equals a.
    a = a - b; // this will act like (a+b) - a, and now an equals b.

It is a clever trick. However, if the addition exceeds the maximum value of the int primitive type as defined by Integer.MAX_VALUE in Java, or if the subtraction is less than the minimum value of the int primitive type as defined by Integer.MIN_VALUE in Java, there will be an integer overflow.

#### Using the XOR method:

Another way to swap two integers without needing a third variable (temporary variable) is using the XOR method. This is often regarded as the best approach because it works in languages that do not handle integer overflows, such as Java, C, and C++. Java has a number of bitwise operators. XOR (denoted by ^) is one of them.

    x = x ^ y; 
    y = x ^ y; 
    x = x ^ y;


## Write down an algorithm for adding a node to a linked list sorted in ascending order(maintaining the sorting property).
An algorithm for adding a node to a link list sorted in ascending order (maintaining the sorting property) is given below:

    - Step 1: Check if the linked list has no value (or is empty). If yes, then set the new node as the head and return it.
    - Step 2: Check if the value of the node to be inserted is smaller than the value of the head node. If yes, place it at the beginning and make it the head node.
    - Step 3: Find the suitable node after which the input node should be added in a loop. To discover the required node, begin at the head and work your way forward until you reach a node whose value exceeds the input node. The preceding node is the correct node.
    - Step 4: After the correct node is found in step 3, insert the node.