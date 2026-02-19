### Training process of neural network
- Forward pass
- Calculate loss function
- Backword pass
- compute gradients 

### Forward pass computation
- Linear transformation
    - z = w.x + b
- Activation:
    - ŷ​=σ(z)
- Loss function
    - L=(ŷ​−y)2
    - Measures difference between predicted and actual output
    - Goal: minimize loss

### Backword pass computation
- After forward pass you have:
    - prediction ŷ
    - true value y
    - loss L
- Now training must answer:
    - How should weights change to reduce loss?
    - if I change w slightly, how much will loss change?
    - Because loss depends on weight indirectly:
        - w → z → ŷ ​→ L
    - We want:
        - ∂L​/∂w
        - To calculate that we use chain rule
        - ∂L/∂w = ∂L/∂ŷ . ∂ŷ/∂z . ∂z/∂w
- After calculating gradient, Now optimizer updates weights:
    - w = w−η.∂L/∂w​


### Autograd
Core componenet of pytorch that provide automatic differentiation for tensors operations. It enable gradient computation, which is essential for training machine learning models using optimized algorithm like gradient descent.