# HackerRank-Quiz
**Part 1**
You need to recover password by meeting following conditions
	- It is a six-digit number
	- The values is withing the range given in your puzzle input
	- Two adjacent digits are the same (like 22 in 122345)
	- Going from left to right, the digits **never decrease**; they only ever increase or stay the same like (111123 or 125679)

Other than the range rule, the following are true:
	- 111111 meets these criteris (doube 11, never decreases)
	- 223450 does not meet these criteris (decreasing pair of digits 50)
	- 123789 does not meet these criteris (no double)

You need to calculate, **how many different passwords** there are within the range given in your puzzle input, which meet these criteria. The range bounds are included in this total, so ong as they satisfy the above criteria.

**Part 2**
After doing part 1, you suddenly remembered one more extra fact about the password **the two adjacent matching digits are not part of a bigger group of matching digits**. Given this extra information, the following are now true:
	- 112233 meets these criteris because the digits never decrease and all repeated digits are exactly two digits long.
	- 123444 no longer meets the criteria (the repeated 44 is part of a larger group of 444)
	- 111122 meets the criteria (even though 1 is repeated more than twice, it still contains a double 22 which satisfies the two adjacent digits rule).
	- 111123 however would **not** meet the criteria, because the 1s are part of a larger group, and there is no other double.
Now, adjust your solution for this extra criteria. 
