# Pascal's Triangle

This project contains a Python implementation of a function that generates Pascal's Triangle.

## Description

Pascal's Triangle is a triangular array of the binomial coefficients that arises in probability theory, combinatorics, and algebra. This project includes a function `pascal_triangle(n)` that returns a list of lists of integers representing the Pascal's triangle of `n` rows.

## Function Specification

The function `pascal_triangle(n)` has the following characteristics:

- It takes an integer `n` as input.
- It returns a list of lists of integers representing Pascal's Triangle up to the nth row.
- If `n` is less than or equal to 0, it returns an empty list.

## Usage

To use this function, import it into your Python script:

```python
from pascal_triangle import pascal_triangle

# Generate Pascal's Triangle with 5 rows
result = pascal_triangle(5)
print(result)
```

This will output:
```
[
    [1],
    [1, 1],
    [1, 2, 1],
    [1, 3, 3, 1],
    [1, 4, 6, 4, 1]
]
```

## Example

Here's an example of how to use the function and print the triangle:

```python
def print_triangle(triangle):
    """
    Print the triangle
    """
    for row in triangle:
        print("[{}]".format(",".join([str(x) for x in row])))

# Generate and print Pascal's Triangle with 5 rows
print_triangle(pascal_triangle(5))
```

This will output:
```
[1]
[1,1]
[1,2,1]
[1,3,3,1]
[1,4,6,4,1]
```

## Repository Structure

- GitHub repository: `alu-interview`
- Directory: `pascal_triangle`
- File: `0-pascal_triangle.py`
