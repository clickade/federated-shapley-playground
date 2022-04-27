# Profit Allocation in Federated Learning | A Playground

*This notebook was developed for my Master's project **"MSAI/21/017 - IMPLEMENTING A GENERAL FRAMEWORK FOR PARTICIPANT’S CONTRIBUTION CALCULATION IN FEDERATED LEARNING"**. The aim of the project is to develop a system that will test the effectiveness of profit allocation using Shapley Value in Horizontal Federated Learning systems. We recommend running this notebook in Google Colab.*

**To run this program, open the `fed-sv-playground.ipynb` in any Jupyter notebook-enabled environment (We recommend Google Colab). Be advised that the program will delete .pt models from previous runs.**

The system has the following customizable functions:

1. Dataset
    - MNIST
    - EMNIST
2. Neural Network Model Size
    - Small MLP
    - Medium MLP
    - Large MLP
3. Contribution Metrics / Reward Function
    - Loss
    - Accuracy
    - F1
4. Individual Client Behaviour
    - Normal
    - Free-rider (No training done)
    - Adversarial (Randomize weights + bias)
5. Client Dataset Distribution (IID)
    - IID
    - Non-IID 1 (Overlapping sample sets)
    - Non-IID 2 (Unequal data distribution)
    - Non-IID 1+2

Once the program completes, it will output the following data:

1. Performance measures: Loss, Acc, F1, Evaluation timing
2. SV rewards per round
3. Client-server training timings
4. User-defined folders with the trained client and server models
