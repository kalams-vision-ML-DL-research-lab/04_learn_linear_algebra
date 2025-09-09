# 04_learn_linear_algebra
# # forming the system of linear equations to solve real world problems.
#i.e
#In a laptop showroom there are laptops with RAM: 4GB, 8GB, and 16GB of different companies: A, B and C. Last week, the showroom sold 2, 1 and 3 laptops with 4GB RAM of companies A, B, and C respectively; 1, 2 and 1 laptops with 8GB RAM of companies A, B, and C respectively; and 2, 3 and 3 laptops with 16GB RAM of companies A, B and C respectively. The pricesof laptops with a particular GB Ram are the same irrespective of the company (i.e., laptops of companies A, B and C with 4GB RAM have the same price; similarly, laptopsof companies A, B and C with 8GB RAM have the same price; and laptopsof companies A, B and C with 16GB RAM have the same price). The owner of showroom earned ₹14, 17 and 18 (in ten thousand) in that week by selling laptop of companies A, B and C respectively.

Using the above information, form the system of linear equations and find the matrix representation of the system of linear equations to find the prices of 1 laptop with 4GB, 1 laptop with 8GM and 1 laptop 16 GB.

sol.
#p, q, r = 4GB, 8GB, 16GB( Columns)

#Owners_urning in a week by selling loptops of company A, B, C = [14, 17, 18]

row1(for company A) = 2p + 1q + 3r = 14 

row2(for company B) = 1p + 2q + 3r = 17 

row3(for company C) = 3p + 1q + 3r = 18 


import numpy as np

df = np.matrix([[2,1,3],[1,2,3],[3,1,3]])

print(df) #representation.

print(df.ndim)

print(df.dtype)

print(df.shape)

print(f"Company_A:{df[0]}=14")

print(f"Company_B:{df[1]}=17")

print(f"Company_C:{df[2]}=18")
