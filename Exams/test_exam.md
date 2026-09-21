# AIA — Test Exam

## Question 1 — Computer Vision Tasks

**1 point**

The company ICU has an automatic access system to ensure that only employees can access their building. A person wishing to enter the building has to show their face to a camera. The acquired image is then matched against an internal database of images of employee faces.

This system is an example application of the general computer vision task of:

* [ ] **a.** Object captioning
* [ ] **b.** Object localization
* [ ] **c.** Object recognition
* [ ] **d.** Semantic segmentation

---

## Question 2 — Classical Computer Vision Pipeline

**1 point**

Bring the steps of the **Classical Computer Vision Pipeline** into the correct order.

> **Note:** The six draggable steps are not contained in the text export.

---

## Question 3 — Classical Computer Vision

**1 point**

Which of the following statements are true?

* [ ] **a.** The feature extraction step maps from pixel space into the output space.
* [ ] **b.** The bag-of-words feature describes spatial relations between image patches.
* [ ] **c.** An intensity histogram feature is rotation invariant.
* [ ] **d.** An intensity histogram feature is illumination invariant.

---

## Question 4 — Fourier Descriptor Normalization

**2 points**

Given is the following Fourier descriptor:

> **Note:** The descriptor figure is missing from the text export.

The following images show different types of normalization applied to the original signal.

Assign to each image the corresponding **invariance** that has been enforced.

> The x-axis shows the frequency \(\mu\). Also note that the frequency range has been shifted.

> **Note:** The four normalization images are missing from the text export.

---

## Question 5 — Fourier Descriptor Invariances

**2 points**

Let \(F\) be a Fourier descriptor. We apply the following transformations and obtain the normalized descriptor \(\tilde F\):

$$
\tilde F(0):=0
$$

$$
\tilde F(\mu):=
\frac{F(\mu)}{|F(2)|}.
$$

Which of the following invariances are enforced by this normalization?

* [ ] **a.** \(\tilde F\) is invariant to translation.
* [ ] **b.** \(\tilde F\) is invariant to scale.
* [ ] **c.** \(\tilde F\) is invariant to noise.
* [ ] **d.** \(\tilde F\) is invariant to mirroring.

---

## Question 6 — Fourier Descriptors

**1 point**

Let

$$
F(\mu), \qquad \mu\in\{0,1,\ldots,69\}
$$

be the Fourier descriptor of some contour.

It is known that

$$
F(0)=293+920i.
$$

How many points were used to describe the contour?

**Answer:** __________

---

## Question 7 — Machine Learning Fundamentals

**1 point**

Which of the following statements are true?

* [ ] **a.** The number of model parameters in logistic regression depends on the number of classes and the input dimensionality.
* [ ] **b.** Gradient descent is only necessary if the error function is non-convex.
* [ ] **c.** Using validation data is only necessary if the error function is non-convex.
* [ ] **d.** We can measure the degree of overfitting using the training data.

---

## Question 8 — Machine Learning

**1 point**

Which of the following statements are true?

* [ ] **a.** Logistic regression, in contrast to linear regression, allows for non-linear classification boundaries.
* [ ] **b.** Model variance can be measured by fitting the model to different subsets of the data.
* [ ] **c.** Optimizing the parameters of a CNN with stochastic gradient descent always leads to the optimal solution.
* [ ] **d.** Data augmentation has a regularization effect.

---

## Question 9 — Transfer Learning

**1 point**

It is common practice to use networks pre-trained on an unrelated dataset for the task at hand.

Why does such an initialization often lead to improved results compared with a random initialization of the network parameters?

* [ ] **a.** Because high-level decision strategies represented in the layers closer to the output layers can be reused.
* [ ] **b.** Because pre-training requires all layers except the final output layer to remain frozen during fine-tuning, thereby preventing overfitting entirely.
* [ ] **c.** Because low-level perceptive capabilities represented in the layers closer to the input are useful across different tasks.
* [ ] **d.** Because transfer learning reduces the number of model parameters at test time.

---

## Question 10 — Backpropagation

**1 point**

Which of the following statements are true?

* [ ] **a.** The memory consumption of backpropagation is proportional to the combined output dimensionalities of the nodes in the network.
* [ ] **b.** For every update step, we need multiple backward passes through the network.
* [ ] **c.** The memory consumption of backpropagation is proportional to the number of trainable parameters in the network.
* [ ] **d.** For every update step, we need multiple forward passes through the network.

---

## Question 11 — Backpropagation

**1 point**

Which of the following statements are true?

* [ ] **a.** Backpropagation allows for efficient optimization of computational graphs with gradient descent.
* [ ] **b.** Backpropagation reduces noise when using stochastic gradient descent.
* [ ] **c.** Optimizing the parameters of a CNN with backpropagation always leads to the optimal solution.
* [ ] **d.** Addition nodes backpropagate their inputs.

---

## Question 12 — Bias, Validation and Model Complexity

**1 point**

Which of the following statements are true?

* [ ] **a.** A small training error suggests sufficient model complexity.
* [ ] **b.** A small validation error suggests good model performance.
* [ ] **c.** A small training error suggests good model performance.
* [ ] **d.** A model with high bias tends to underfit the data.

---

## Question 13 — Hough Transform

**1 point**

Given is an image showing the Hough voting space for line detection, containing **three maxima**.

> **Note:** The image is missing from the text export.

Which geometric object(s) could cause this?

* [ ] **a.** Circle
* [ ] **b.** Triangle
* [ ] **c.** Square
* [ ] **d.** Parallelogram

---

## Question 14 — Hough Line Parameterization

**1 point**

Let

$$
(x,y)=(2,10)
$$

be a 2D point.

Which of the following lines parameterized by \((\theta,\rho)\) intersect this point?

* [ ] **a.** \((\theta,\rho)=(0,2)\)
* [ ] **b.** \((\theta,\rho)=(0.75\pi,-10)\)
* [ ] **c.** \((\theta,\rho)=(0,10)\)
* [ ] **d.** \((\theta,\rho)=(0.5\pi,2)\)

---

## Question 15 — Generalized Hough Transform

**1 point**

Which statements about the **Generalized Hough Transform (GHT)** are true?

* [ ] **a.** In order to apply R-tables at a position \((x,y)\), one needs to calculate the orientation of the corresponding gradients.
* [ ] **b.** Translating the template object does not change the R-table.
* [ ] **c.** A single R-table is invariant to scale and rotation of the template.
* [ ] **d.** R-tables can deal with partial occlusions.

---

## Question 16 — R-Table Transformation

**1 point**

Given is the following R-table of a template:

| Orientation \(\theta\) | Displacement     |
| ---------------------- | ---------------- |
| \([0,45)\)             | \((1,2); (3,4)\) |
| \([45,90)\)            |                  |
| \([90,135)\)           | \((5,6); (7,8)\) |
| \([135,180)\)          | \((9,10)\)       |

What is the corresponding R-table with scale

$$
s=2
$$

and a counter-clockwise rotation of

$$
\theta=180^\circ?
$$

### a.

| Orientation \(\theta\) | Displacement     |
| ---------------------- | ---------------- |
| \([0,45)\)             | \((5,6); (7,8)\) |
| \([45,90)\)            | \((9,10)\)       |
| \([90,135)\)           | \((1,2); (3,4)\) |
| \([135,180)\)          |                  |

### b.

| Orientation \(\theta\) | Displacement             |
| ---------------------- | ------------------------ |
| \([0,45)\)             | \((-2,-4); (-6,-8)\)     |
| \([45,90)\)            |                          |
| \([90,135)\)           | \((-10,-12); (-14,-16)\) |
| \([135,180)\)          | \((-18,-20)\)            |

### c.

| Orientation \(\theta\) | Displacement         |
| ---------------------- | -------------------- |
| \([0,45)\)             | \((4,2); (8,6)\)     |
| \([45,90)\)            |                      |
| \([90,135)\)           | \((12,10); (16,14)\) |
| \([135,180)\)          | \((20,18)\)          |

### d.

| Orientation \(\theta\) | Displacement     |
| ---------------------- | ---------------- |
| \([0,45)\)             | \((1,2); (3,4)\) |
| \([45,90)\)            |                  |
| \([90,135)\)           | \((5,6); (7,8)\) |
| \([135,180)\)          | \((9,10)\)       |

---

## Question 17 — Deformable Parts Model

**1 point**

How are objects, or their parts, localized within images in the **Deformable Parts Model**, when using a dense feature space such as HOG?

* [ ] **a.** Using Hough forest regression
* [ ] **b.** Classifying patches at multiple locations
* [ ] **c.** The output of the SVM is a location
* [ ] **d.** Using a codebook and Hough voting

---

## Question 18 — Implicit Shape Model

**1 point**

Bring the steps of the **training phase of the Implicit Shape Model** into the correct order.

> **Note:** The five draggable steps are not contained in the text export.

---

## Question 19 — Convolutional Filters

**1 point**

What is the result of an increased number of filters in a convolutional layer of a Convolutional Neural Network?

* [ ] **a.** Decrease in output dimensionality of the layer
* [ ] **b.** Higher abstraction capabilities of the layer
* [ ] **c.** Increase in output dimensionality of the layer
* [ ] **d.** Increased number of features the layer can potentially respond to

---

## Question 20 — Pooling

**1 point**

What are effects of **max-pooling layers** in Convolutional Neural Networks?

* [ ] **a.** Dimensionality reduction
* [ ] **b.** Translation invariance
* [ ] **c.** Loss of spatial/relational information
* [ ] **d.** Translation equivariance

---

## Question 21 — Convolutional Layer Parameters

**1 point**

The input tensor to a convolutional layer has dimensionality

$$
(H\times W\times C)=(32,32,12).
$$

The output tensor has dimensionality

$$
(H'\times W'\times C')=(16,16,28).
$$

The filter size is

$$
(3,3).
$$

How many trainable parameters does the layer have, considering **only the kernel tensor and no bias**?

**Answer:** __________

---

## Question 22 — Convolutional Stride

**1 point**

The input tensor to a convolutional layer has dimensionality

$$
(148,148,7).
$$

The output tensor has dimensionality

$$
(74,74,42).
$$

The filter size is

$$
(3,3).
$$

What is the stride of the layer?

**Answer:** __________

---

## Question 23 — Histograms and Entropy

**2 points**

Given are four image patches.

Drag and drop the matching **intensity histograms** and **entropy values** to the correct image patch.

Available items:

* Histogram a
* Histogram b
* Histogram c
* Histogram d
* Entropy a
* Entropy b
* Entropy c
* Entropy d

> **Note:** The image patches, histograms, and entropy values are missing from the text export.

---

## Question 24 — Saliency

**1 point**

Which is the **most salient image patch**, given the entropy values above and using the method by **Kadir et al.** introduced in the lecture?

* [ ] **a.** a
* [ ] **b.** b
* [ ] **c.** c
* [ ] **d.** d

---

## Question 25 — Entropy and Saliency

**1 point**

Why is the entropy of the distribution of intensity values alone **not sufficient as a measure of saliency**?

* [ ] **a.** Saliency can only be measured in color images.
* [ ] **b.** The distribution of intensity values does not contain spatial information.
* [ ] **c.** Uniformly distributed intensity values always lead to high entropy.
* [ ] **d.** Because regions with a single intensity value are salient.

---

## Question 26 — Sequential Models

**2 points**

Given is the following one-hot encoding:

$$
\text{"0"}\mapsto(1,0,0)
$$

$$
\text{"1"}\mapsto(0,1,0)
$$

$$
EOS\mapsto(0,0,1).
$$

A sequential model \(f\) has been trained using this encoding.

During inference, the model generates the following outputs:

| Input      | Output              |
| ---------- | ------------------- |
| \(f(x_1)\) | \((0.1,0.8,0.1)\)   |
| \(f(x_2)\) | \((0.9,0.05,0.05)\) |
| \(f(x_3)\) | \((0.6,0.4,0.0)\)   |
| \(f(x_4)\) | \((0.2,0.7,0.1)\)   |
| \(f(x_5)\) | \((0.1,0.3,0.6)\)   |

What is the corresponding sequence?

$$
\_\_\_,\quad
\_\_\_,\quad
\_\_\_,\quad
\_\_\_,\quad
\_\_\_
$$

---

## Question 27 — Backpropagation Through Time

**2 points**

Given is the RNN shown below.

What is the derivative with respect to \(x_1\) if you apply **backpropagation through time** for the sequence

$$
(x_1,x_2,x_3)?
$$

Assume

$$
a=1,
\qquad
x_1=1,
\qquad
x_2=4,
\qquad
x_3=5,
$$

and the initial state

$$
h_0=0.
$$

> **Note:** The RNN diagram is missing from the text export.

**Answer:** __________

---

## Question 28 — Probability Density Estimation

**1 point**

Which of the following models/methods estimate a distribution over the data?

* [ ] **a.** Maximum likelihood estimation
* [ ] **b.** Generative Adversarial Networks
* [ ] **c.** Parzen Windows
* [ ] **d.** (Restricted) Boltzmann Machines

---

## Question 29 — Maximum Likelihood Estimation

**3 points**

Assume a computer vision system is observing an industrial production process for errors.

We measure the number of errors in a certain time interval. Let

$$
X=\{2,8,4,2,6\}
$$

be the measurements.

We model the probability of observing \(k\) errors using a **Poisson distribution**:

$$
P(k)=\frac{\lambda^k}{k!}e^{-\lambda}.
$$

What is the maximum likelihood estimate

$$
\lambda_{\mathrm{MLE}}
$$

given the measurements?

> Round the solution to two decimal places.

**Answer:** __________

---

## Question 30 — Bayesian Inference

**3 points**

Two probabilistic models are given by their respective parameters

$$
\theta\in\{\Omega_1,\Omega_2\}.
$$

The likelihoods of these models on data \(D\) are

$$
P(D\mid\theta=\Omega_1)=0.52
$$

and

$$
P(D\mid\theta=\Omega_2)=0.58.
$$

Additionally, we have the prior probabilities

$$
P(\theta=\Omega_1)=0.53
$$

and

$$
P(\theta=\Omega_2)=0.47.
$$

What is the posterior probability

$$
P(\theta=\Omega_1\mid D)?
$$

> Round to four decimal places.

**Answer:** __________

---

## Question 31 — Discriminant Functions

**1 point**

Which of the following are **discriminant functions**?

* [ ] **a.**

  $$
  g_i(x)=p(x\mid\omega_i)
  $$

* [ ] **b.**

  $$
  g_i(x)=P(\omega_i)
  $$

* [ ] **c.**

  $$
  g_i(x)=\sqrt{p(x\mid\omega_i)P(\omega_i)}
  $$

* [ ] **d.**

  $$
  g_i(x)=P(\omega_i\mid x)
  $$

---

## Question 32 — Generative Models and Self-Supervised Learning

**1 point**

Which of the following statements are true?

* [ ] **a.** The goal of energy-based SSL is to map images with small mean-square distance in pixel space to the same region of the representation space.
* [ ] **b.** Contrastive learning uses data augmentation to generate a gradient.
* [ ] **c.** Variational autoencoders learn an approximation of the data distribution.
* [ ] **d.** Self-supervision objectives are necessarily regression tasks.

---

## Question 33 — Generative Adversarial Networks

**1 point**

For each of the following statements about **Generative Adversarial Networks (GANs)**, indicate whether it is **True** or **False**.

| Statement                                                                                                                                    | True | False |
| -------------------------------------------------------------------------------------------------------------------------------------------- | :--: | :---: |
| The generator network learns the empirical probability function of the dataset.                                                              |  [ ] |  [ ]  |
| All GANs require a labeled dataset, i.e. a dataset consisting of tuples \((x,y)\), where \(x\) is the input and \(y\) is the desired output. |  [ ] |  [ ]  |
| CycleGANs train two generators and two discriminator networks simultaneously.                                                                |  [ ] |  [ ]  |
| The computation of backpropagation for the generator network is independent of the discriminator.                                            |  [ ] |  [ ]  |
