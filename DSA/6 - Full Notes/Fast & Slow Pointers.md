2025-09-20 14:47

Status:
#baby 

Tags: 
#GrokkingTheCodingInterview 

# Fast & Slow Pointers

**What is it?**
- This is also known as a hare and tortoise algorithm
- We have two pointers which move at different speeds through a data structure
	**Example:**
		- One friend walks one lap per hour
		- One friend walks two laps per hour
		- If the (data) structure is circular, the fast friend (pointer) will catch up or lap the slow friend (pointer)

**Why do we use it?**
- To detect if we're in a cycle
- We can find positions such as the middle of a list, or the start of a cycle.

**Where do we use it?**
- Given a linked list, determine if it has a cycle
- Find the middle node of a list in one pass
- Determine the length of a cycle
- Reordering or splitting a linked list

**How do we use it?**
- Initialise both pointers to the head of the list
- In each iteration:
	- Move slow pointer by 1 node
	- Move fast pointer by 2 nodes
- If the fast pointer ever becomes null, it means the list isn't cyclical
- If slow meets fast, there is a cycle or special condition we're looking for

##### Special Algorithms
**Floyd's Tortoise and Hare Algorithm:**
- When our pointers meet, we're in a cycle
- Reset the slow pointer to the head of the list
- Move both pointers one at a time now
- When we next meet, we're at the start of the cycle
# References
[[Grokking the Coding Interview]]
https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/introduction-to-fast-slow-pointers-pattern