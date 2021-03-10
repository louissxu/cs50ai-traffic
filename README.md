# Traffic

### CS50 AI Exercise 5

Experimentation using tensor flow to create convolutional neural network for categoridation of German Traffic Sign Recognition Benchmark (GTSRB) dataset.

Usage:
```python
python traffic.py data_directory [model.h5]
```

Starting naive model:
- 2D Convolution: 32, (3, 3), relu
- Max pool: (2, 2)
- Neural network:
  - 128 nodes, relu, dropout 0.5
  - 43 output nodes, softmax
- **Accuracy 0.0561**

Final model:
- 2D Convolution: 32, (3, 3), relu
- Max pool: (2, 2)
- 2D Convolution: 64, (3, 3), relu
- Neural network:
  - 128 nodes, relu, dropout 0.5
  - 128 nodes, relu, dropout 0.5
  - 43 output nodes, softmax
- **Accuracy 0.9678**