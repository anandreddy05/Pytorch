# Pytorch

Pytorch is an open source machine learning framework developed by Facebook.

## Key Highlights

**Pythonic Design**: Pytorch feels native to Python making it easier for python developers. It integrates seamlessly with Python libraries like Numpy, Scipy and more.

**Tensor Operations**: Pytorch tensors are similar to numpy arrays but can run on GPUs, making operations significantly faster

**Automatic Differentiation (Autograd)**: Pytorch's aotograd module simplifies gradient computation, making it easy to implement and debug complex models.

**TorchScript for Production**: Enables models to be exported for deployment.

## Computation Graph

A computation graph is a graphical representation of operations and data in your neural network. It's how PyTorch keeps track of all the operations you do on tensors, so it can automatically compute gradients during backpropagation.

### How it works

Every time you perform an operation on a tensor, PyTorch builds a node in the graph.

Each node represents a tensor or an operation (like addition, multiplication, matrix multiplication, etc.).

Edges in the graph represent how outputs of one operation are inputs to another.

When you call .backward(), PyTorch traverses this graph in reverse to compute gradients — this is the backpropagation step.
