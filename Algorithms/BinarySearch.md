# Binary Search 

## Overview
Search through a sorted array to find an element 

- Time Complexity -  **O(Log(N))** 
- Space Complexity **O(1)**  : Only 3 variables are being created

## General algorithm 
Lets say we have a sorted array **nums** and we want to find **target**

```cpp
int leftptr = 0 ; 
int righptr = nums.size();
while(leftptr < rightptr){
    int mid = leftptr + rightptr /2 ; 
    if(nums[mid] < target){
        leftptr = mid;
    }
    if(nums[mid] > target){
        rightptr = mid;
    }
    if(nums[mid] == target){
        return 
    }
}
```