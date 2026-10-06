# Toy Models of Superposition Demo

An interactive, in-browser demo of the toy model from
[Toy Models of Superposition](https://transformer-circuits.pub/2022/toy_model/index.html) (Elhage et al., 2022).

**Live demo:** https://sbel2.github.io/toy-models-of-superposition-demo/

Built by **Yan (Stella) Si**, BU CDS PhD.

## What it shows

- **The network:** x′ = ReLU(WᵀWx + b) with n features and m < n hidden neurons. Click an input to toggle it and hover any node to see its arithmetic.
- **Hidden space:** each column of W drawn as an arrow, with the polytope the features form (pentagon, square pyramid, octahedron, …) and whether the model is in superposition.
- **W, WᵀW and b:** the learned weights, interference and biases.
- **Training data:** samples from the sparse input distribution set by S.

The model trains live in the browser with Adam (4,000 steps × 1,024 fresh examples, best of 4 random starts). Everything is in a single `index.html` with no build step.
