# Matrix Calculator

A desktop application developed for an **Advanced Linear Algebra** coursework project.

The calculator provides a graphical interface for entering matrices and performing four linear algebra operations: diagonalizability checking, LU decomposition, the power method, and singular value decomposition.

## Features

- **Diagonalizability Check:** Calculate eigenvalues and eigenvectors and check whether a square matrix is diagonalizable.
- **LU Decomposition:** Compute lower and upper triangular matrices using Doolittle's method.
- **Power Method:** Approximate a dominant eigenvalue and its corresponding eigenvector.
- **Singular Value Decomposition:** Calculate the left singular vectors, singular values, and transposed right singular vectors.
- **Matrix Input:** Enter a matrix row by row and reuse it across operations.

Diagonalizability checking, LU decomposition, and the power method require square matrices. SVD also supports rectangular matrices.

## Tools

- **Python**
- **NumPy** for numerical calculations
- **Tkinter** for the desktop interface
- **Jupyter Notebook** for standalone implementations and examples

## Project Structure

| Folder | Description |
| --- | --- |
| `Matrix Calculator/` | Desktop application and calculation modules |
| `Diagonalizable Matrix/` | Diagonalizability notebook and documentation |
| `LU Decomposition/` | LU decomposition notebook and documentation |
| `Power Method/` | Power method notebook and documentation |
| `Singular Value Decomposition/` | SVD notebook and documentation |

The desktop application starts from `tkinterSatya.py`, which imports the four calculation modules stored in the same folder.

## How to Run

Use Python with Tkinter available, then install NumPy:

```sh
pip install numpy
```

From the repository root, launch the application:

```sh
cd "Matrix Calculator"
python tkinterSatya.py
```

## Usage

1. Select **Insert/Change your Matrix**.
2. Enter each row as space-separated numbers, pressing **Enter** after every row.
3. Click **Submit Matrix**.
4. Return to the main menu and select an operation.
5. Click the calculation button to display the result.

Use **Reset Console/Matrix** before entering a replacement matrix.

## Notes

- LU decomposition does not use pivoting, so some matrices requiring row exchanges cannot be processed.
- The power method uses a maximum of **10 iterations** and a tolerance of **0.01**. Convergence is not guaranteed for every matrix.
- Calculations use floating-point arithmetic, so results may contain small numerical differences.

## Authors

**Computer Science and Statistics — BINUS University**

- Anthony
- Hazel Z. Adityo
- Marcell Prasetyo
- Satya D. Padmakumara
- Siddharta R. Wallace
