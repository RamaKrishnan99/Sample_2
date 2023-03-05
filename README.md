# Sample_2
# Python3 program to find largest
# x such that p*x divides n!

# Returns largest power of p that divides n!
def largestPower(n, p):
	
	# Initialize result
	x = 0

	# Calculate x = n/p + n/(p^2) + n/(p^3) + ....
	while n:
		n /= p
		x += n
	return x

# Driver program
n = 2022; p = 7
print ("The largest power of %d that divides %d! is %d\n"%
								(p, n, largestPower(n, p)))
		
# This code is contributed by Shreyanshi Arun.
