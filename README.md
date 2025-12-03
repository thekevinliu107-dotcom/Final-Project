# Final-Project
CISC 121 Final Project

# Algorithm Name
  VisualBinarySearch is the name of this Python app where users are able to interact with their chosen list of numbers to find their target value!
  It will visually show (through text) how binary search works; the pointers are there to show the list getting narrowed down.
  When left pointer = right pointer then user's target value was successfully found! Otherwise not found.



## Demo video/gif/screenshot of test
  For this section I decided to test a bunch of edge cases
  
![Screenshot 2025-12-03 003504](https://cdn-uploads.huggingface.co/production/uploads/692f27dd343168c4a7eef6e9/YRyrxU4Kxv52HseeSXUaC.png)
This tested if when a list is already sorted and target value is not contained in the original list, if the program still functions.
It ran perfectly and the value was not found even when the list was prematurely sorted.

![Screenshot 2025-12-03 003559](https://cdn-uploads.huggingface.co/production/uploads/692f27dd343168c4a7eef6e9/q3HJJdRgEklY5L3ZdI00F.png)
This tested a reverse sorted list and if it can find a duplicate number. Safe to say, it found the first appearance of it perfectly.

![Screenshot 2025-12-03 003627](https://cdn-uploads.huggingface.co/production/uploads/692f27dd343168c4a7eef6e9/df0HjSpDLfaxF4pH6PZG8.png)
This was probably the most important edge case testing. It tested if a empty list was validated before the binary search.
It actually failed as you can see the code still ran which is not ideal since I wanted it to invalidate and send a "Please enter valid input" message.
You will see that I have fixed this in the current version.



## Problem Breakdown & Computational Thinking
  - Decomposition
    - First accept user inputs
    - Conversion of user's inputs into an integer list
    - Make sure the list is sorted, if not use the sorted function
    - Set up left and right pointers
    - Through multiple steps, calculate middle index
    - Compare this middle index to user's inputted target
    - Adjust the pointers (search range)
    - Display each step

  - Pattern Recognition
    - Binary search repeats same pattern
    - Looks at middle element, compares, removes half, repeated until left pointer = right pointer (meaning middle index matches target value)

  - Abstraction
    - Completely ignore if the user's numbers represent anything, just treat as values
    - Show only important steps like the output, that is the pointers, middle index and value
    - Hides the math from user's, they don't need to know how the middle value is found and reached

  - Algorithm Design
    - The inputs will be user's numbers obviously separated by spaces and their target value
    - Processing will be conversion of input strings to integers
    - Then sort the list
    - Then actually do the binary search
    - Finally store each step in a list
    - Outputs wil be a sorted array, each step number, pointers, searching left or right half, success/fail message



## Steps to Run
  1. Open the URL which navigates you to the VisualBinarySearch space
  2. Click on app located near the top right
  3. Now all you have to do is insert your input into the textbooks
  4. Click submit
  5. Outputs should be displayed accordingly



## Hugging Face Link
  https://huggingface.co/spaces/KevinSpace/VisualBinarySearch/tree/main



## Author & Acknowledgment
  Kevin Liu
  
  CISC 121 Student
  
  Completed as CISC 121 final project
