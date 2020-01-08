# README.md
### Task 1: BST<br>
In my binary search tree code, struct node(line 4 ~ line 10) is how I create each node with id, age, left node and right node.<br>
The function insert(line 14 ~ line 33) can insert a node to a binary search tree with input BST, and the id, age of the node you want to insert.<br>
The function search(line 36 ~ line 47) can search a node's age in a BST with its id.<br>
The function remove(line 51 ~ line 78) can remove a node with the given id from the BST.<br>
The function test(line 80 ~ line 88) is just for me to print out the id's of each node in the BST to test my code.<br>
In my main function, I initialize the BST as figure 1 in the sample (line 92 ~ line 101), than add two nodesto the BST(line 103 ~ line 104), than delete a node from BST(line 106), than search the node with id=13 and print its result(line 108 ~ line 109).<br>
### Task 2: AVL<br>
##### Q1<br>
As the definition of an AVL tree, tree (a) is not an AVL tree because the balance factor of node 8 is -2. Tree (b) is an AVL tree because all of balance factors of its nodes are between -1 and 1. Tree (c) is not an AVL tree because the balance factor of node 9 is 2.<br>
##### Q2<br>
The BST from Task 1 is not an AVL tree because the balance factor of the node with id=10 is 2.<br>
##### Q3<br>
The approach I use in this task is RL, I first use LL on the Node with id=14 and then use RR on the Node with id =10. To test my code, the function level(line 46 ~ line 67) and the function factor(line 69 ~ line 85) are used to calculate each node's factor. And the function isAVL(line 139 ~ line 160) calls them to test if the balance factor of all the nodes in the tree are between -1 and 1. After using the function rebalance, the tree is balanced.<br>
### Task 3: Concurrent search<br>
##### Q1<br>
In the code, the funtion traversal(line 85 ~ line 97) is to use thread to print the pre-order tree traversal. The function inside the threads is print which print the id of the node. the function traversal also print out the age of the patient with id=6 once there is a match.
