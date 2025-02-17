# Read input from the user and store it as an integer
x = int(input())

# Determine the sign of the number (negative or positive)
# If x is negative, sign will be -1, otherwise it will be 1
sign = -1 if x < 0 else 1

# Make x positive (work with absolute value)
x = abs(x)

# Initialize revNum to 0. This will hold the reversed number
revNum = 0

# Loop to reverse the digits of the number
while x > 0:
    # Get the last digit of x
    r = x % 10
    # Remove the last digit from x
    x = x // 10
    # Add the digit to revNum, shifting its digits to the left
    revNum = (revNum * 10) + r

# Restore the original sign to the reversed number
revNum *= sign

# Check if revNum is within the 32-bit signed integer range
# If it's outside the range, print 0 (overflow or underflow)
if revNum > 2*31 - 1 or revNum < -2*31:
    print(0) 
else:
    # Print the reversed number if it's within the valid range
    print(revNum)
