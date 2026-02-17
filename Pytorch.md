### Tensor
- A datastrcuture
- Specialized multi-dimensional array designed to for mathematical and computational efficency.
- Rank 0: 
    - Scaler: 0 dimensional tensor
    - Represent a single value
    - Example 5 or 3.14
- Rank 1:
    - Vectors / array: 1 dimensional tensor
    - Example: 1D vector embeddings
    - [1.24, 1.5, 0.89]
- Rank 2: Matrix
    - Matrices: 2 dimensional array.
    - Example: Gray scale image can be represented as 2 dimensional array
    - [[1,2,3], 
    [2,3,4]]
- Rank 3: 
    - Adds a third dimension also used for staking data
    - Example: Colored image

### Why tensors are used?
- Tensor enable efficient mathematical computation (addition, multiplication, dot product etc) necessary for neural network operation.

- Data like image, video and text can be represented as tensors.

### Where are tensors used?
- For storing training data(image, text, video)
- Learnable parameter of neural network (weight and bias) are stored in tensor.
- Neural network involve operation like matrices multiplication and dot product are performed on matrices.
- In training process, in forward pass tensor flow through the process. Gradient, represented as tensors are calculated during backword pass.