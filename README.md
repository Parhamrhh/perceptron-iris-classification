# Perceptron Implementation on the Iris Dataset 

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)

This project demonstrates a **manual implementation of the Perceptron learning algorithm** from scratch, applied to a binary classification task using the classic **Iris flower dataset**.

The goal is to find a linear decision boundary that separates two species of Iris based on their physical measurements.

## Project Overview

The Perceptron is one of the earliest and simplest machine learning algorithms used for **binary classification**.  
In this project:

- Loaded and explored the Iris dataset  
- Prepared the data for binary classification  
- Implemented the perceptron update rule  
- Trained the modeled until convergence  
- Visualized decision boundaries and results  

The implementation is fully done in a **Jupyter notebook**.  

## Methodology 

The Perceptron is a fundamental, single-layer linear classifier. It learns by iteratively adjusting its weights and bias only when it makes a mistake.

For each misclassified sample, the model updates its weights ($w$) using the following rule:

$$w_{new} = w_{old} + \eta \cdot (y_{\text{true}} - y_{\text{pred}}) \cdot x$$

Where:
* $\mathbf{w}$: The weight vector.
* $\mathbf{\eta}$ (learning\_rate): A constant controlling the step size.
* $\mathbf{y_{\text{true}}}$: The actual label (1 or -1).
* $\mathbf{y_{\text{pred}}}$: The model's predicted label.
* $\mathbf{x}$: The input feature vector.

Training continues until either a maximum number of epochs is reached or the model achieves **convergence** (zero classification errors).


## Dataset & Preprocessing

The project utilizes the **Iris Dataset**. For the Perceptron's binary nature, the data was preprocessed:

* **Species Selected:** Only *Setosa* and *Virginica* were used (100 samples total).
* **Target Labels:** Converted to numerical values: **1** (Setosa) and **-1** (Virginica).
* **Features Selected:** Sepal Length and Sepal Width for easy 2D visualization.


## Results

The model was trained with a learning rate ($\eta$) of 0.3.

1.  **Decision Boundary:** The algorithm successfully found a linear hyperplane separating the Setosa and Virginica species, demonstrating their linear separability using the selected features.
2.  **Error Convergence:** The misclassification error dropped to zero quickly, confirming that the model successfully learned the optimal weights.


### Requirements

To run the notebook locally, you will need Python installed along with the following libraries:

```
pip install numpy pandas matplotlib seaborn mlxtend
```

### Usage

1.  **Clone the repository:**

```
 git clone https://github.com/parhamrhh/perceptron-iris-classification.git
```

2.  **Run the Jupyter Notebook**: Open the `Perceptron_Algorithm_on_the_Iris_Dataset.ipynb` file in your preferred notebook environment and follow the instructions to preprocess data, visualize it, and train the model.


## Contributing

Contributions, issues, and feature requests are welcome! Feel free to suggest improvements to the implementation, visualizations, or documentation.

