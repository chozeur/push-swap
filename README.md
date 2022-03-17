# Rules
Given a list of single random numbers, the aim of push_swap is to sort that list.
We can use two stacks in order to sort the given numbers. Considering the two stacks A & B, here are the actions we can apply on each stack.
|Name|Function|
| --- | --- |
|sa (swap A)|Swap the first 2 elements at the top of stack A. Do nothing if there is only one or no elements.|
|sb (swap B)| Swap the first 2 elements at the top of stack B. Do nothing if there is only one or no elements.|
|ss|sa & sb at the same time|
|pa (push A)|Take the first element at the top of B and put it at the top of A. Do nothing if b is empty|
|pb (push B)|Take the first element at the top of A and put it at the top of B. Do nothing if b is empty|
|ra (rotate A)|Shift up all elements of stack A by 1. The first element becomes the last one.|
|rb (rotate B)|Shift up all elements of stack B by 1. The first element becomes the last one.|
|rr|ra & rb at the same time|
|rra (reverse rotate A)| Shift down all elements of stack A by 1. The last element becomes the first one.|
|rrb (reverse rotate B)| Shift down all elements of stack B by 1. The last element becomes the first one.|
|rrr|rra & rrb at the sme time|

The objective is to finaly get the list sorted increasingly in A, using the less number of actions we can.
