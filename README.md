# Black-Scholes Neural Network Approximation  

This project is focusing on approximating the nonlinear Black-Scholes (BS) formula for financial option derivatives using neural networks.  

## Project Overview  
The goal is to develop, optimize, and evaluate a neural network model that approximates the BS formula. The project explores various neural network architectures, activation functions, optimizers, and hyperparameters to achieve minimal Mean Squared Error (MSE) and robust generalization.  

### Key Objectives:  
1. Experiment with varying neural network architectures (shallow and deep).  
2. Analyze the impact of activation functions, neuron counts, optimizers, and epochs.  
3. Select the best model based on MSE and convergence properties.  
4. Validate the model’s robustness through random data splits.  

---

## Project Structure  
- **`code/`**: Contains Python notebooks (`.ipynb`) and scripts for training and testing the model.  
- **`data/`**: Includes sample datasets and preprocessed data for model training.  
- **`reports/`**:  
  - Final report explaining the experiments and results.  
  - Plots showcasing convergence, error metrics, and comparisons.  
- **`README.md`**: This file.  

---

## Methodology  
### Part A: Parameter Exploration  
1. **Layers**: Shallow vs. Deep networks (1 to 3 layers).  
2. **Activation Functions**: `ReLU`, `Sigmoid`, `Tanh`.  
3. **Neuron Counts**: Experiments with 10, 50, and 100 neurons.  
4. **Optimizers**: `Adam`, `RMSprop`, and SGD with Momentum.  
5. **Epochs**: Evaluated performance over 100, 500, and 1000 epochs.  

### Part B: Best Model Selection  
The optimal model configuration is selected based on:  
- Mean Squared Error (MSE) on the test set.  
- Convergence properties across training and validation losses.  

### Part C: Robustness Testing  
- The best model is retrained with a random split of training, validation, and test sets.  
- Results are compared to ensure generalization.  

---

## Results  
- Best Configuration:  
  - **Layers**: 1  
  - **Activation Function**: `Tanh`  
  - **Neurons**: 50  
  - **Optimizer**: `Adam`  
  - **Epochs**: 1000  
- **Test Set MSE**: 0.0000996  
- Random Split MSE: 0.0001350  

These results demonstrate the neural network’s ability to effectively approximate the Black-Scholes function while maintaining robustness across splits.  

