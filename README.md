# primeornot
from math import sqrt

def is_prime(n):
    if n == 1:
        return False
    for i in range(2, int(sqrt(n) + 1)):
        if n % i == 0:
            return False
    return True

n = int(input())

if is_prime(n):
    print(n, "is PRIME")
else :
    print(n, "is NOT Prime")
