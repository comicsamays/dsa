2025-10-27 12:33

Status:
#baby 
Tags:
#GrokkingTheCodingInterview 
# Cyclic Sort

**What is it?** 
A pattern where we sort an array of numbers in a given range by placing the number in their respective array index

**Where do we use it?**
- When we have an array of numbers in a given range
- When we have duplicates / missing numbers to identify

**Why do we use it?**
- It's more efficient for this specific niche of number sorting

**How do we use it?**
- Use the fact the input has numbers from 1 to n
- Place each number at its respective index e.g.
	- 1 at index 0
	- 3 at index 2
	- and so on...
- Once sorted, iterate through the array to find the indices of all missing numbers.

# References
[[Grokking the Coding Interview]]
https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/introduction-to-cyclic-sort-pattern