# HackerRank-Data-Structures
Arrays - Hourglass Problem

# Question

Given a  6* 6 2D Array, find the hourglass pattern with max sum.

# Code:

Complete the hourglassSum function below.
def hourglassSum(arr):
    sumList = []
    for i in range(0,4):
       for j in range(0, 4):
        sumElement_hourglass = arr[i][j] + arr[i][j+1] + arr[i][j+2] + arr[i+1][j+1] + arr[i+2][j] + arr[i+2][j+1] + arr[i+2][j+2]
        sumList.append(sumElement_hourglass)
    return max(sumList)


