# Adversarial Machine Learning
Course Research Project, EECS127 Optimization Models in Engineering, UC Berkeley
## Introduction
This repo contains code, dataset (MNIST) for this course research project. I trained a provably robust ReLU-based neural network handwritten digit classifier against norm-bounded perturbations.
The adversarial examples were generated using the **F**ast **G**radient **S**igned **M**ethod (FGSM). By considering the **convex outer polytope** of the ReLU, a robustness certificate was derived. I dualized the original network and perturbation constraints and get the dual network, which is more computable.
The dual network was trained with the robustness certificate, achieving significantly higher accuracy compared to the original network under norm-bounded perturbations. I also  attack it with natural perturbations (rotation, translation), which are not norm-bounded and found its robustness is still not enough.  
Click [here](https://drive.google.com/file/d/1qrBYxeFOyc96KV6VeUv9m3JZPyQzYhXA/view?usp=sharing) to view my report. Please include your reason in the message.   
## What's in the files 
`adversarial.ipynb`: Code for training a robust classifier.


`extension.ipynb`: Code for attacking the robust classifier with other adversarial samples like rotation and translation.


`./data`: MNIST dataset


`proj_adversarial_prob`: Problems of the project, done by EECS127 staff.