def addFactor(factors, f):
    if (f not in factors):
        factors[f] = 1
    else:
        factors[f] += 1

import math
                
def factorize1(n):
    factors = {}
    sqrtn = math.floor(math.sqrt(n))
    for i in range(2, sqrtn + 1):
        while (n % i == 0):
            addFactor(factors, i)
            n = n // i
    if (n > 1):
        addFactor(factors, n)
    return factors 

import time
start = time.time()
n = (2 ** 18) - 1
for i in range(2, n + 1):
    factorize1(i)
end = time.time() 
print("실행시간:", (end - start))   
    
