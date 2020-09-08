# Linear Algebra Review

1. Span

   The span of **v**  and **w** is the set of all their linear combinations.

   a**v** + b**w** , a and b vary over all real numbers.

2. linear dependent 

   **u** = a**v** + b**w**, for some values of a and b.

3. basis

   the basis of a vector space is a set of linearly independent vectors that spans the full space.

4. linear transformation

   lines remain lines; origin stay at the same space.

   grid lines remain parallel and evenly spaced.

   matrix expression: 第一列代表 **i** 变换后的坐标，第二列表示 **j** 变换后的坐标，以此类推。左乘对应的矩阵可以得到向量变换后的结果。

   matrix multiplication: 从右向左，分别是 transform 的顺序。不同个线性组合的复合。**order matters!**

5. determinant

   the transformed area (2d) / volume (3d) are scaled by the determinant 

   negative: flipping the space / 右手定则变左手定则
   $$
   det(M_1M_2) = det(M_1)det(M_2)
   $$

6. rank of A

   number of dimensions in the output

7. column space of A

   set of all possible outputs A**v** / span of columns 矩阵的列张成的空间

   因此，更精确的rank的定义是列空间的维数。

   零向量永远都在列空间中，因为线性变换必须保持在原点位置不变且一直在原点。

   满秩的矩阵只有原来的原点会变成零向量，非满秩可能有一条过原点的线/过原点的面。

8. Null space of A

   变换后落在原点的向量的集合。

9. Gaussian elimination

10. row echelon form


