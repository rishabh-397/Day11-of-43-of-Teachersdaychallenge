# Day11-of-43-of-Teachersdaychallenge

. A. George and Accommodation
Problem Description: George and Alex want to live in the same room. Given n rooms, where each room i has pi people living and a capacity of qi people, count how many rooms have enough free space for both George and Alex. (i.e., qi - pi >= 2).

Key Idea/Logic:

Read the number of rooms n.

Initialize a counter for suitable rooms to 0.

Loop n times:

In each iteration, read the current number of people p and the capacity q for a room.

Calculate the number of free spots: free_spots = q - p.

If free_spots is greater than or equal to 2 (meaning enough space for George and Alex), increment the counter.

After the loop, print the final count.

Time Complexity: O(N) where N is the number of rooms, as each room's input is processed in constant time.

Space Complexity: O(1) (only a few variables needed).

Example:
Input:

3
1 10
0 10
10 10
Output: 2
Explanation:
Room 1: 10 - 1 = 9 free spots (>=2, count++)
Room 2: 10 - 0 = 10 free spots (>=2, count++)
Room 3: 10 - 10 = 0 free spots (<2, skip)
Total suitable rooms: 2

A. Word
Problem Description: Vasya wants to change the case of letters in a given word s so that it either consists entirely of lowercase letters or entirely of uppercase letters. The goal is to change as few letters as possible. If a word has an equal number of uppercase and lowercase letters, convert all to lowercase.

Key Idea/Logic:

Read the input word s.

Count the number of uppercase letters and lowercase letters in s.

Compare the counts:

If uppercase_count > lowercase_count, convert the entire word s to uppercase.

Otherwise (lowercase_count >= uppercase_count), convert the entire word s to lowercase.

Print the corrected word.

Time Complexity: O(L) where L is the length of the word, as you iterate through the word once to count and once to convert.

Space Complexity: O(L) for storing the word (or O(1) if modifications are in-place and input is read character by character).

Example:
Input: HoUse
Output: house
Explanation: 'H', 'U' (2 uppercase), 'o', 'u', 's', 'e' (4 lowercase). Lowercase count is greater, so convert to "house".

Input: ViP
Output: VIP
Explanation: 'V', 'P' (2 uppercase), 'i' (1 lowercase). Uppercase count is greater, so convert to "VIP".

Input: maTRIx
Output: matrix
Explanation: 'T', 'R', 'I' (3 uppercase), 'm', 'a', 'x' (3 lowercase). Counts are equal, so convert to "matrix".

