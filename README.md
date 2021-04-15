# bott-theorem

# the content of this project is essentially the function coh, all the rest is preparatory to it. Its arguments are a string and a list. The string determines the Dynkin type of the homogeneous vartiety and it must be either A, B, C, D, E or F. The list represents the weight of the bundle of which we compute the cohomology, expressed in a basis of fundamental weights, and it must have integral coefficients

# the output is a string [x,y] where x is the dimension of the unique nonzero cohomology group, and y is the degree of such cohomology

# example: consider the Grassmannian G(2,4) with tautological bundle U and quotient bundle Q. 
# The following code computes the cohomology of the tensor product of U^* with Q(-2), which is zero in every degree except for 1, where it is one-dimensional

# input:
import bott

print(bott.coh('A', [1, -2, 1]))

# output: 
[1, 1]

