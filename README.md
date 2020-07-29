# Deep-Learning-Coursera-Specialisation
This repository has all of the Coursera Deep-Learning specialization assignments taught by Andrew N G with a brief description of the topics by me.
Below, I will give a breif description of each lab assignments which might give a generic idea to someone who isn't able to do the course on Coursera. 
I geniunely reccomend you to take up the course if you are interested in deep learning, as Andrew is one of the best at what he does. 


Week1. 
There are no programming assignments on week1. This is a introductory week into the course and talks about the application and scope of deep learning. The activation fuctions 
are discussed about. The Sigmoid and the ReLu/Rectified linear unit functions are briefly described.

Week2.(Logistic_Regression_with_a_Neural_Network_mindset_v6a)
This week starts off more technically by introducing the problem of logistic regression. For someone who isn't famialr with what logistic regression is, it is just a fanct word 
for binary classification. Breaking down a step further, binary classification is the process of differentiating 2 classes( between the picture of a cat and something else). The 
output of this classification problem is a 1 or a 0. 1 indicating that the picture is indeed that of a cat and 0 being that of a noncat. 

Consider any random image. The basic bullding blocks of an image are pixels. The number of pixels in the row*column gives the size or the pixel count of an image. Say a square shaped
image has a length of 64 pixels and breadth of 64 pixels. The total number of pixels would then be (64*64=4096). Another detail of a "COLOURED" image are the red, greed and blue(RGB) values
Each pixel has a particular R, G and B value. In deep-learning we use all this from an image as data for the model. So finally we end up wit (64*64*3) values from the image we have 
considered above. They are arranged as a column vector [ R1 G1 B1 R2 G2 B2.....].T. These are the features of the image. So now we have a single image and its (12288) features 
arranged as a column vector (12288,1) dimension. The number of features is associated with the term nx. Hence the matrix will have dimenstion (nx,1). If we have m images, then the
dimension of the imput matrix would be (nx,m).

The data is given pre-optimized to us in the course. Each picture has the image x associated with a label y which is 1 for cat and 0 for non-cat.

The sigmoid activation is clearly explained and the intricacies of a simple logistic regression procedure are elaborated. A few more terms like the loss function/cost function and 
gradient descent are explained in detail. It's best you audit the course and go through these sections of the video lecture. 

The most importart part of this week starts with the introduction of the forward and backward propagation process with the help of computational graphs, and anyone without a backing in calculus have a lesson which exceptionally
elaborates on the calculus parts of this course. VECTORIZATION is a must to understand!! Andrew also explains the reduncancy for loops cause. Using the python numpy package, vectorization
makes it a cakewalk on the CPU/GPU. 


Week3.(Planar_data_classification_with_onehidden_layer_v6c)
In the week 2 assignment we implemented a simple neural network/ probably the most simply neural network. In this week a denser neural network is implemented. The math and the matrix 
dimensions at each step are elaborated. Andrew insists on the importance of matrix dimensions and how it helps in debugging. To be honest, I felt it to be really useful too. What basically
happens in a dense NN the same as that of the logistic reg example, but the activation of the previous layer is used as an input to the next layer. This, I feel is the main difference
between machine learning and Deep learning. In DL the math happens BTS. I like it! Lesser math to deal with. 

The ReLu, Sigmoid, Tanh and the leaky ReLu and their viability as activations at difference layers of the network are explained. For example, using a sigmoid at the last later in a classification problem makes a lot of sense. The derivatives of the 
activations are also given which help in backprop later. Gradient descent in a neural network with more than one layer is generalized. A super important aspect of why NN of more than 1 layer
shouldn't be initialized by zeros is clearly explained by Andrew. A more off beat random gaussian initiaization with a scale-down factor is used. 

Week4.(Building_your_Deep_Neural_Network_Step_by_Step_v8a,Deep+Neural+Network+-+Application+v8)
In the final week of the course we work through a deep neural network of 4 layers (indexed from zero including the iinput and output layers). The first layer has 5 units, second 5, third 3 and the 1 output layer.
The dimensionality of each layer is also mathematically defined. Forward prop and back prop with the usage of Cache( a dictonary which stores a few input values neccassary during backprop) is elaborated. This was 
the hardest part for me in this course. It takes some time to understand. Atleast it did for me.




