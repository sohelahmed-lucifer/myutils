# Single neuron
z = np.dot(W, X) + b
sigmoid = 1 / (1 + np.exp(-z))
relu = np.maximum(0, z)
z, sigmoid, relu
# Q3a
n_features = 10
layer1 = 5
layer2 = 3
output = 1
params_q3a = (n_features*layer1 + layer1) + (layer1*layer2 + layer2) + (layer2*output + output)
# Q3b (generalized)
def count_params(n, m, s, t):
    return (n*m + m) + (m*s + s) + (s*t + t)

params_q3a, count_params
