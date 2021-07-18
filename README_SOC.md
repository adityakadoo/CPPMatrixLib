# This is the README file that was to be submitted for SOC

# This main branch only contains all the code that I have contributed to this project. 
Because of a few merge conflicts this branch does not have all the code from all of the contributors.

As our workflow was mainly from feature branches of individual forks [adityakadoo/CPPMatrixLib/feature/polynomial](https://github.com/adityakadoo/CPPMatrixLib/tree/feature/polynomial) to develop banches of those forks [adityakadoo/CPPMatrixLib/develop](https://github.com/adityakadoo/CPPMatrixLib/tree/develop) then to the develop branch of the main repository [relaxxpls/CPPMatrixLib/develop](https://github.com/relaxxpls/CPPMatrixLib/tree/develop), this main branch [adityakadoo/CPPMatrixLib](https://github.com/adityakadoo/CPPMatrixLib) doesn't have much use. So I've decided to showcase my contributions here.

Below I have given detailed week-wise log of all the work that I did during the project

# Week 0
We spent time first understanding the code for [matrix.hpp](https://github.com/adityakadoo/CPPMatrixLib/blob/main/include/matrix/matrix.hpp) and [matrix_utility.hpp](https://github.com/adityakadoo/CPPMatrixLib/blob/main/include/matrix/matrix_utility.hpp) that was written by our mentor.

We had to make a my_gauss_elim.cpp(this file got deleted unfortunately) file that performed the Gauss elimination method to compute the Row Echelon form of a given matrix using the above mentioned libraries as a test while applying for the project.

# Week 1
After an introductory meet we were given resources for understanding Git, time and space complexity and other DSA basics.

We also had to go through divide and conquer algorithms such as merge sort(recursive and iterative), quick sort, binary search and stassen's multiplication. We also solved a few CP problems from codeforces, codechef, spoj and leetcode to better understand these concepts.

Then we had to implement the Strassen's Matrix Multiplication algorithm in the [matrix.hpp](https://github.com/adityakadoo/CPPMatrixLib/blob/main/include/matrix/matrix.hpp) file to improve complexity from O(n^3) to O(n^2.8). But as this algorithm is recursive, it takes a lot of time for smaller inputs (n<10,000) and thus we didn't include it in the end.

# Week 2
We were to add unit-tests to our repository using [googletests](https://github.com/google/googletest) and Cmake framework. So we spent time learning cmake and googletest syntax.

Impelemented googletests and cmake in a dummy folder to get a better understanding.

# Week 3
Made extensive tests for matrix libraries. I worked on making parameterized tests and made a library [test1.hpp](https://github.com/adityakadoo/CPPMatrixLib/blob/main/tests/matrix/test1.hpp) to test different funtions for a variety of inputs and implemented it using [test1.cpp](https://github.com/adityakadoo/CPPMatrixLib/blob/main/tests/matrix/test1.cpp).

We solved a few CP problems that used the concepts and functions implemented using our matirx libraries such as Binary exponentiation, Gaussian XORs and Linear recurrence relations.

# Week 4
The work for making testing libraries continued for me and also helped to point out bugs in the [include/matrix/matrix.hpp] such as an error in operator*= function for matrix multiplication and precision error for operator== function.

I resolved the bug with operator== funtion by making new equality_integral() and equality_floating_point() funtions to handle the two cases separately.

We also learned about trees, graphs and implementing DP and solved a few CP problems on these topics.

# Week 5
This week we were assingned different tasks individually or in teams of two. I was given the task to program the [polynomial.hpp](https://github.com/adityakadoo/CPPMatrixLib/blob/main/include/polynomial/polynomial.hpp) and [polynomial_utility.hpp](https://github.com/adityakadoo/CPPMatrixLib/blob/main/include/polynomial/polynomial_utility.hpp).

I made the above mentioned header files and implemented basic arithmetic operations(addition,subtraction,scalar multiplication and naive polynomial multipilcation), evaluation operation, differentiation, etc.

I also had to implement the divide and conquer version of polynomial multiplication, Karatsuba multiplication. But it also being recursive was slower for smaller test cases thus was not added to [polynomial.hpp](https://github.com/adityakadoo/CPPMatrixLib/blob/main/include/polynomial/polynomial.hpp) but kept in [polynomial_utility.hpp](https://github.com/adityakadoo/CPPMatrixLib/blob/main/include/polynomial/polynomial_utility.hpp).

I also made similar parameterizes testing library [test1.hpp](https://github.com/adityakadoo/CPPMatrixLib/blob/main/tests/polynomial/test1.hpp) to test the different funtions for polynomial class and implemented it using [tests/polynomial.test1.cpp](https://github.com/adityakadoo/CPPMatrixLib/blob/main/tests/polynomial/test1.cpp).

# Week 6
We learned about fast fourier transform and number theortic transform through resources. Also saw how the polynomial multiplication(O(n^2) to O(nlogn)) and evaluation(O(n) to O(logn)) can be made faster.

We were to implement these in our polynomial class but this isn't done yet(at the time of submission).