When assigning to an array, we may include a set of square brackets following the name of the variable to be assigned to whose contents signify multiple locations. If the value on the right of the assignment operator is a scalar, then that value will be assigned to all of the locations specified by the square brackets on the left. For example, consider the following code:

```py-cell
import numpy as np

a = np.array([[0, 0, 0], [0, 0, 0], [0, 0, 0]])
a[:, 1] = 5 # Set the middle column to 5
a[::2, ::2] = 10 # Set the four corners to 10

print(a)
```