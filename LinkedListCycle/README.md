I use Floyd's Cycle Detection Algorithm,also called the two-pointer technique.

The algorithm uses two pointers:`slow` and `fast`.

The `slow` pointer moves one node at a time,while the `fast` pointer moves two nodes at a time.

If the linked list has a cycle,the fast pointer will eventually catch up with the slow pointer.When `slow == fast`,it means that there is a cycle.

If `fast` reaches `null` or `fast.next` is `null`,there is no cycle in the list.

For example:

3 -> 2 -> 0 -> -4
     ↑         |
     └─────────┘
     
Time Complexity
The time complexity is O(n).
Here,n is the number of nodes in the linked list.

The two pointers move through the linked list,and each node is visited only a limited number of times.Therefore,the number of operations grows linearly with the number of nodes.
The space complexity is O(1) because the algorithm only uses two pointers and does not need extra data structures.
