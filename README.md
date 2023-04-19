
## **Image Classification using Forward-Forward Algorithm**

| Name | ID | Responsibility |
| --- | --- | --- |
| Tristan Leduc | A20517874 | Model Implementation, report result |
| Ishrat Jahan Ananya | A20516799 | Model Implementation, report result |

📌 Paper Reference: Hinton, Geoffrey. "The forward-forward algorithm: Some preliminary investigations." *arXiv preprint arXiv:2212.13345*
 (2022).

📌 Download the model weights at : https://drive.google.com/drive/folders/1X__0cUcL5BGJNnFs1e-mGsgE7hz9YHxc?usp=sharing
📌 Refer to the final report in the doc folder for final results and new approach
### Problem statement
---

The problem addresses a novel approach for neural networks which is more computationally efficient than the current backpropagation method. This experimental method, called Forward Forward algorithm, stages the supervised image classification task as a learning exercise to differentiate between ‘positive’ and ‘negative’ images. This allows the network to learn more quickly and effectively as it replaces the backward pass in the backpropagation method with two forward passes. The objective of the project is to analyze the performance of this unconventional approach on small scale datasets and report its feasibility. 

### Approach

---

Along the course of this project, we will implement several neural networks embodying the concept of forward forward weight update. We will build a simple fully connected network using forward forward and assess its performance when compared with the standard backpropagation approach on simple visual classification tasks. Then, we will further investigate the ways to improve on the forward forward method including :

- exploring the ways to corrupt data in different manners to see if it allows the model to better discriminate between negative data (generated data) and actual training data (positive data)
- figuring out ways to combine the forward forward mechanism with convolution and more generally the concept of shared weights.

If successful, this segment of the study could lead us to overcome the limitations of forward forward networks and to try more intricate network architectures. 

### Data

---

For the purpose of this project we will evaluate our custom model on two small datasets: Fashion MNIST and CIFAR-100. The choice of datasets depended heavily on the nature of the images. Fashion MNIST dataset serves as an alternative to the MNIST dataset used in the paper. It has the same structure with 70,000 samples for benchmarking ML models. Its relatively straight forward with the object of interest being easily identifiable in the centre of the image. The second dataset, in other words, the ‘hard dataset’ introduces variability and detection bottlenecks due to complex backgrounds in the image. The purpose of using Cifar100 is simply to evaluate the models performance on images that are historically known to perform better with CNNs over simple FCNs.

### References

---

1. paper: [https://arxiv.org/abs/2212.13345](https://arxiv.org/abs/2212.13345)
2. FashionMNIST dataset: [https://www.kaggle.com/datasets/zalando-research/fashionmnist](https://www.kaggle.com/datasets/zalando-research/fashionmnist)
3. CIFAR100: [https://www.cs.toronto.edu/~kriz/cifar.html](https://www.cs.toronto.edu/~kriz/cifar.html)
