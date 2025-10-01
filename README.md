# Single neuron
z = np.dot(W, X) + b
sigmoid = 1 / (1 + np.exp(-z))
relu = np.maximum(0, z)
z, sigmoid, relu
