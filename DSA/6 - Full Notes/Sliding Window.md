2025-10-15 14:16

Status: #baby 

Tags: #GrokkingTheCodingInterview 

# Sliding Window

**What is it?** 
Say we want to perform calculations on 5 elements at a time in an array, instead of accessing 5 elements each iteration, we remove the first element of our interval and add the next element to the overall value.

**Where do we use it?**
When we're asked to find or calculate something from a list of sublists / an array of subarrays of fixed size, particularly when we can contextually only perform one pass of the array

**Why do we use it?**
In a normal brute-force approach, for a window of 5 elements, as we iterate over the array, we are evaluating the whole window repeatedly which is inefficient. Sliding window reduces the amount of necessary calculations


**How do we use it?**
Have a variable for:
- index of the start of the sliding window
- The sum or calculation of all the elements in the window
- a results array for our results
- K - represents the size of each subarray we are looking at
For each element in the array / list:
- Add the next element to the sum / calculation
- If the element index >= K - 1, we should start sliding
	- Calculate the sum / average / aggregate value we need and append to results array
	- remove the value of the start of the sliding window
	- increment the index of the start of the sliding window
Return the results array
# References
[[Grokking the Coding Interview]]
https://www.designgurus.io/course-play/grokking-the-coding-interview/doc/introduction-to-sliding-window-pattern