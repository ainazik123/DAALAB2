I use two pointers to go through the two sorted linked lists.

First,I create a dummy node and use a `current` pointer to build the result list.Then I compare the values of the current nodes of `list1` and `list2`.

If the value in `list1` is smaller or equal,I add that node to the result and move `list1` forward.Otherwise,I add the node from `list2` and move `list2` forward.

I continue comparing the nodes until one of the lists becomes empty.After that,I connect the remaining part of the other list to the result.

For example:
List 1: 1 -> 2 -> 4
List 2: 1 -> 3 -> 4

Result: 1 -> 1 -> 2 -> 3 -> 4 -> 4 

Time Complexity
The time complexity is O(n + m).
Here,n is the number of nodes in the first list and m is the number of nodes in the second list.

Each node from both lists is checked only once.Therefore,if the first list has n nodes and the second list has m nodes, the total number of operations is proportional to n + m.
The space complexity is O(1) because I only use a few pointers and do not create a separate new list.
