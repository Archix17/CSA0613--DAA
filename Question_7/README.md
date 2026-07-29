# Question 7

## Title
Brute-Force Approach to Find the Farthest Pair of Delivery Points

## Objective
To identify the farthest pair of delivery points by checking the distance between every possible pair of coordinates using the brute-force approach.

## Pseudocode

BEGIN

Input n (number of delivery points)

FOR i = 0 to n-1
    Read x[i] and y[i]
END FOR

maxDistance ← 0

FOR i = 0 to n-1
    FOR j = i+1 to n-1
        distance ← √((x[i]-x[j])² + (y[i]-y[j])²)

        IF distance > maxDistance THEN
            maxDistance ← distance
            point1 ← i
            point2 ← j
        END IF
    END FOR
END FOR

Display point1, point2 and maxDistance

END

## Algorithm
1. Read the number of delivery points.
2. Input the coordinates of all delivery points.
3. Initialize the maximum distance to zero.
4. Compare every pair of points.
5. Calculate the Euclidean distance for each pair.
6. Update the maximum distance whenever a larger distance is found.
7. Display the farthest pair and the maximum distance.

## Time Complexity
**O(n²)**

## Space Complexity
**O(n)**
