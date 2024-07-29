# Gi  Fusion Tech Assessment 

This repository contains solutions to various SQL problems. The focus is on solving challenges related to identifying patterns in data.

## Problems and Solutions

### 1. Longest Substring Without Repeating Characters

**Description**:  
Given a string `s`, find the length of the longest substring without repeating characters.

**Example**:
- **Input**: `s = "abcabcbb"`
- **Output**: `3`
- **Explanation**: The longest substring without repeating characters is "abc", which has a length of 3.

**Solution**:  
The solution involves using a sliding window approach with a dictionary to track the indices of characters. The algorithm updates the window size based on the presence of repeating characters to ensure it only contains unique characters.


### 2. Numbers That Appear at Least Three Times Consecutively

**Description**:  
Given a table `Logs` with columns `id` and `num`, find all numbers that appear at least three times consecutively.

**Example**:
- **Input**:
    | id | num |
    |----|-----|
    | 1  | 1   |
    | 2  | 1   |
    | 3  | 1   |
    | 4  | 2   |
    | 5  | 1   |
    | 6  | 2   |
    | 7  | 2   |
- **Output**:
    | ConsecutiveNums |
    |-----------------|
    | 1               |
- **Explanation**: The number 1 appears consecutively at least three times.

**Solution**:  
The solution uses self-joins to compare consecutive rows in the `Logs` table. It checks if a number appears in three consecutive rows and selects distinct numbers meeting this criterion.



