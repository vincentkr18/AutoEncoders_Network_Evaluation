## Generic auxiliary tasks to learn features that help regularize the network using Auto-encoder

Autoencoders play a basic role in supervised and
unsupervised learning and in deep learning architectures for
transfer learning and one of a kind tasks. For two main reasons,
the reduction of dimensionality has been an important subject of
analysis in academia. Firstly, large volume of data resulting in
computing costs and becomes difficult to handle. Also, mapping
from higher dimensional to lower dimensional data without losing
much information removes redundant dimensions in our dataset.
Also, impact of the data sizes on the trained model results in
high variance in model performance . In this paper, an approach
of how autoencoders will be used for three different dataset
which were collected from different domains will be discussed
along with data description, experiments, impact of data sizes,
limitations, challenges and their results will be presented. The
results of the stacked autoencoder will also be compared with a
standard algorithm and its performances will be discussed


#### EXPERIMENTS

For all the three datasets, an individual autoencoders will
be trained first to find the best parameter for the autoencoder
algorithm to replicate out input data. Then the encoder part
which is the compressed learned features of all the input will
stacked with a neural network to predict the classes of the
target. But this steps will be experimented by taking smaller
to all data points in the dataset. Their performace will be
measured for different sample proportions and the autoencoder
bottleneck neuron counts.The following sppraches will be
taken. Firstly training a autoencoder and passing the well
trained auto encoder as input to an artificial neural network
and predict the target variable.

An autoencoder is a neural network that learns efficient data
coding by replicating the structure of its input.   The objective type of network consists of two parts:  
**Encoder:** Encoder part of the network deforms the input
into a depiction of latent space. The encoding functionality
h= f (x) can represent it.  
**Decoder:** Decoder segment is intended to recreate the
input from the real representation of latent space. A decoding
function r= g (h) can represent it.  
Autoencoders are expected to keep as many information
as possible whenever an input runs through the encoder and
then the decoder, but they are still trained to have different
nice properties in the new display. It is a feed-forward neural
network that aims to minimize the loss function from the
output which is the difference between the actual input and
the output Once the loss is minimized it means that once
autoencoder has been trained.This implies that once properly
trained autoencoders are quite accurate and it will be hard to
generalize data sets other than those for which they have been
trained

### Results

**Breast Cancer:**
|Sample Size |Accuracy | AUC | F1 Score | Recall | Precision |
| ----------- |----- |----- |----- |----- |----- |
|20% |0.792 |0.81 |0.79 |0.79 |0.86|
|40% |0.905 |0.91 |0.91 |0.91 |0.92|
|60% |0.958 |0.96 |0.96 |0.96 |0.96|
|80% |0.947 |0.95 |0.95 |0.95 |0.95|
|100% | 0.966 |0.97 |0.97 |0.97| 0.97|

**Model Results**
 | Model |  Precision |  Recall  | F1   Score | 
 | ------| ----- |----- |----- |
 | Logistic Regression  | 0.96 |  096  | 0.96 | 
 | Support Vector machine |  0.93  | 0.93 |  0.93 | 
 | K-Nearest Neighbours  | 0.93  | 0.93 |  0.93 | 


The codes for three datasets are present outside their individual directory and the names have been listed below

Dataset1 - Breast Cancer Code -->  breast-cancer-Autoencoder_final.ipynb, 
Dataset2 - Census Income Code -->  Census_autoencoder_final.ipynb, 
Dataset3 - Santander customer satisfaction Code -->  santander_autoencoder.ipynb


