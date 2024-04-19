# Python-Computational_Mathematics

## Assignment-01 (Interpolation and Lagrange Interpolation)

### Interpolation

Interpolation is a method in mathematics and computational science used to estimate values between known data points. It is particularly useful when we have a set of discrete data points and need to estimate the value of a function at points that lie between these data points. Interpolation is commonly used in various fields such as numerical analysis, signal processing, computer graphics, and scientific computing.

### Lagrange Interpolation

Lagrange interpolation is a polynomial interpolation method that constructs a polynomial function that passes through a given set of data points. It is named after the mathematician Joseph-Louis Lagrange.

### Lagrange Interpolation Formula

Given \( n \) data points \( (x_i, y_i) \), where \( i = 0, 1, 2, ..., n-1 \), the Lagrange interpolation polynomial \( P(x) \) is given by:

\[
P(x) = \sum_{i=0}^{n-1} y_i \cdot l_i(x)
\]

where \( l_i(x) \) are the Lagrange basis polynomials defined as:

\[
l_i(x) = \prod_{j=0, j \neq i}^{n-1} \frac{x - x_j}{x_i - x_j}
\]

### Explanation of Code

The provided Python code demonstrates Lagrange interpolation to estimate pressure values at given temperature points. Here's a breakdown of the code:

- **`lagrange_interpolation` Function**: This function implements Lagrange interpolation. It takes three parameters:
  - `x`: Array of x-coordinates (temperature points).
  - `y`: Array of y-coordinates (pressure points).
  - `x_val`: Value at which interpolation is to be performed (temperature at which pressure is to be calculated).

- **Data Points**: The code defines arrays `temperature` and `pressure` representing known temperature-pressure data points.

- **User Input**: The user is prompted to input a list of temperatures at which pressure is to be calculated.

- **Interpolation**: The Lagrange interpolation function is called with the temperature and pressure data along with the user-input temperature points.

- **Plotting**: The code plots the known data points as dots and the interpolated points as a continuous line.

- **Visualization**: The resulting plot visualizes the pressure-temperature relationship using Lagrange interpolation.

### How to Use

To use this code, follow these steps:

1. Ensure you have Python installed on your system.
2. Install the required libraries: `numpy` and `matplotlib`.
3. Copy the provided code into a Python file (e.g., `interpolation_example.py`).
4. Run the Python script.
5. Enter the temperatures at which you want to interpolate pressures when prompted.
6. View the plotted graph showing the original data points and the interpolated points.

![Screenshot (135)](https://github.com/suraj-soni-04/Python-Computational_Mathematics/assets/154866411/31686eef-c401-4645-a0a0-2262556ffaa0)

<hr>

## Assignment-02 (Gauss Elimination)

### Gaussian Elimination

Gaussian elimination is a method used to solve systems of linear equations. It operates by systematically eliminating variables from the equations until a solution is found. This technique is fundamental in various fields such as mathematics, physics, engineering, and computer science.

### How Gaussian Elimination Works

1. **Forward Elimination**: The method starts by converting the system of equations into an equivalent triangular system through a series of row operations. This process simplifies the system and makes it easier to solve.

2. **Back Substitution**: Once the triangular system is obtained, the solution is found by solving for each variable one by one, starting from the bottom and working upwards.

## Explanation of Code

The provided Python code implements Gaussian elimination to solve a system of linear equations of the form \( AX = B \). Here's a breakdown of the code:

- **`gauss_elimination` Function**: This function takes two parameters:
  - `a_matrix`: Coefficient matrix \( A \) of the system.
  - `b_matrix`: Right-hand side vector \( B \) of the system.

- **Input Validation**: The function validates the dimensions of the input matrices to ensure they are compatible for Gaussian elimination.

- **Forward Elimination**: The code performs forward elimination with partial pivoting to convert the coefficient matrix into an upper triangular form.

- **Back Substitution**: After obtaining the upper triangular form, the code performs back substitution to find the solution vector \( X \).

- **Printing Solution**: Finally, the code prints the solution vector \( X \) to the console.

### How to Use

To use this code, follow these steps:

1. Ensure you have Python installed on your system.
2. Copy the provided code into a Python file (e.g., `gaussian_elimination.py`).
3. Run the Python script.
4. Enter the values for the coefficient matrix when prompted.
5. Enter the values for the constant matrix when prompted.
6. View the solution vector printed to the console.

![Screenshot (134)](https://github.com/suraj-soni-04/Python-Computational_Mathematics/assets/154866411/21987b02-5a97-4bb6-bfa4-163d984fef21)

