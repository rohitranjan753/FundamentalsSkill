# ALGORITHMS 10 Interview Question

## Write down an algorithm for adding a node to a linked list sorted in ascending order(maintaining the sorting property).

- An algorithm for adding a node to a link list sorted in ascending order (maintaining the sorting property) is given below:

    - Step 1: Check if the linked list has no value (or is empty). If yes, then set the new node as the head and return it.

    - Step 2: Check if the value of the node to be inserted is smaller than the value of the head node. If yes, place it at the beginning and make it the head node.

    - Step 3: Find the suitable node after which the input node should be added in a loop. To discover the required node, begin at the head and work your way forward until you reach a node whose value exceeds the input node. The preceding node is the correct node.

    - Step 4: After the correct node is found in step 3, insert the node.


## Write an algorithm for counting the number of leaf nodes in a binary tree.

- An algorithm for counting the number of leaf nodes in a binary tree is given below:

    - Step 1: If the current node is null, return a value 0.

    - Step 2: If a leaf node is encountered, that is, if the current node's left and right nodes are both null, then return 1.

    - Step 3: Calculate the number of leaf nodes recursively by adding the number of leaf nodes in the left subtree by the number of leaf nodes in the right subtree.