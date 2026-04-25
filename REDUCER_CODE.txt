import sys
current_product = None
total = 0

for line in sys.stdin:
product, price = line.strip().split("\t")
price = float (price)
if current_product == product:
total += price
else:
if current_product:
print(f" {current_product} \t{total}")
current_product = product
total = price

if current_product:
print(f" {current_product}\t{total}")
