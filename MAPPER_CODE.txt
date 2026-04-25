for line in sys.stdin:
data = line.strip().split(",")
if len(data) == 6:
product = data [1]
price = float(data [4])
print(f" {product} \t{price}")

import sys
