2025-10-16 13:29

Status: #baby 

Tags: #GrokkingTheCodingInterview 

# Merge Intervals
**What is it?**
- There are 6 ways two intervals can relate to each other
![[Pasted image 20251016133125.png]]

We use this whenever we work with interval based questions

**How do we use this?**
- Sort our list of intervals based on their starts
- Initialize an empty merged list to store the merged intervals
- Set an initial interval to start
- Iterate through the rest of the intervals
	- If there is overlap, merge them by updating the end of the previous interval to be the maximum of both ends.
	- If they do not overlap, add the previous interval to the merged intervals list
		- Update the current interval to be the next interval in the list
- When the loop is complete, add the previous interval one last time to the merged intervals list
# References
[[Grokking the Coding Interview]]
https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/introduction-to-merge-intervals-pattern