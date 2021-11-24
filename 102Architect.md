# Geometric transformations
* In graphics programming , objects can usually:
  * Move
  * Change size
  * Turn
  * Change place
  * etc

# Translation
 V(i,j)
 P'(x) = P(x) + i
 P'(y) = P(y) + j

# scaling

P'(x) = m*P(x)
P'(y) = P(y)*n

#rotation

P'(x) = cos(teta) *P(x) -sin(teta)*P(y)
P'(y) = sin(teta)*P(x) etc


# Reflection over an axis

P'(x) = cos2(teta) * P(x)

# Matrices
*  A matrice is a two dimensional array of values
*  Matrices can repesent points in 2D, 3D, etc

# Addition of two matrices
* To be added, 2 matrices must have the same dimensions
* The resulting matrix has the same dimensions.

# Mulgtiplication of two matrices

* 2 Matrices can be multiplied by the number of colums of the first on in the same as the number of rows of the second one.
* The resulting matrix has the number of rows of the first one


# How to multiply matrices

3
6
2

321


# Homogeneous coordinates

* In graphics programming, we use homogeneous coordinates to easaly compute transformations.
* A point (x,y) is represented as 3x1 matrix with a third "coordinate" equal to 1:
* x
* y
* 1


# Translation
x'......./10i\\...../x\\ \
y'.=..| 01j |..*.| y|  \
1.......\\001/.....\\1/


# Scaling

(x'/y'/1) = (m00/0n0/001)

# Rotation centered

# Reflexion

# End goal:
T is a transaltion matric, and R a rotation matrix
P'=T*P
P" = R*P' = R*(T*P) = (R*T) * P

# 102 Architect:
Inputs:
* x,y: original coordinates
* At least one information

Outputs:
* Yhr mztrix of the composed transformation
* The resulting transformed coordinates
  
Using a library that calculates matrixes is forbidden


# Suggested bonuses:
* Graphical interface showing transformation of several points/figures
* Additional transformations:
  * Shear mapping
  * Projection
  * ...
* 3D