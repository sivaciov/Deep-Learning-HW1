# Deep Learning HW1: Nearest Neighbor Classifier

This repository contains the implementation of a **Nearest Neighbor Classifier** as part of Homework 1 for a Deep Learning course. The goal of this task is to classify data points based on their proximity to labeled training examples in feature space.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Usage](#usage)
  - [Installation](#installation)
  - [Running the Script](#running-the-script)
- [Example Output](#example-output)
- [Dependencies](#dependencies)
- [License](#license)

## Overview
The **Nearest Neighbor Classifier** is a simple, yet effective machine learning model that assigns labels to test samples based on the labels of their closest neighbors in the training set. This implementation focuses on:

1. Efficient computation of pairwise distances.
2. A basic but functional classification pipeline for academic purposes.
3. Clear and well-documented code for educational use.

## Features
- **Distance Metrics:** Implements Euclidean distance for determining nearest neighbors.
- **Customizable Parameters:** Easily adjust the number of neighbors to consider (`k`) for classification.
- **Lightweight and Simple:** Pure Python implementation with minimal dependencies.

## Usage

### Installation
Clone the repository to your local machine:

```bash
git clone https://github.com/sivaciov/Deep-Learning-HW1.git
cd Deep-Learning-HW1
```

### Running the Script
Ensure you have Python 3.6 or later installed. Run the `nearest_neighbor_classifier.py` script as follows:

```bash
python nearest_neighbor_classifier.py --train_file <path_to_training_data> --test_file <path_to_test_data> --k <num_neighbors>
```

#### Command-line Arguments
- `--train_file`: Path to the training dataset (CSV or compatible format).
- `--test_file`: Path to the test dataset (CSV or compatible format).
- `--k`: Number of nearest neighbors to consider (default is 1).

Example:
```bash
python nearest_neighbor_classifier.py --train_file data/train.csv --test_file data/test.csv --k 3
```

## Example Output
After running the script, the classifier will output:
1. Predicted labels for the test set.
2. Overall accuracy of the classifier.

Sample output:
```
Accuracy: 92.3%
Predicted Labels: [1, 0, 1, 1, 0, ...]
```

## Dependencies
This implementation uses only the Python standard library. No additional dependencies are required.

Optional (for better CSV handling):
- `numpy`

Install using:
```bash
pip install numpy
```

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to modify the code to suit your specific needs or extend it further for advanced use cases!
