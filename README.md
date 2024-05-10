# DeepFool-Attack-and-Defense-using-Adversarial-Training-and-Defensive-Distillation

## Introduction

Adversarial attacks pose a significant threat to the reliability of deep learning models. DeepFool is one such attack that perturbs inputs to mislead models into making incorrect predictions. This project aims to study the vulnerability of a model trained on the MNIST dataset to DeepFool attacks and to bolster its robustness using adversarial training and defensive distillation.

## Usage

For this project, start by preparing the MNIST dataset, which you can conveniently download using TensorFlow's built-in functions. Once you have the dataset ready, proceed to train a deep learning model on it. You have the flexibility to choose any architecture that suits your preferences, such as a Convolutional Neural Network (CNN) or a Multi-Layer Perceptron (MLP).

Next, implement the DeepFool attack on the trained model. DeepFool is categorized as a white-box attack, which means it relies on access to model gradients. After successfully implementing the attack, augment your training data with adversarial examples generated using DeepFool. With this augmented dataset, re-train the model to improve its robustness against adversarial attacks.

Following adversarial training, apply defensive distillation to further enhance the model's resilience. Defensive distillation involves training a distilled model on softened logits (probabilities) of the original model. This technique aims to make the model less sensitive to small perturbations in input data.

Finally, evaluate the robustness of the original model, the adversarially trained model, and the defensively distilled model against the DeepFool attack. Measure various metrics such as accuracy and adversarial accuracy to gauge their performance under adversarial conditions. Visualize the results to gain insights into the effectiveness of each defense mechanism against adversarial attacks.
