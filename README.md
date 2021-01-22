# Devnagari Handwritten Character Recognition using custom activation functions for CNN

Designed and Implemented Handwritten Devnagari Character recognition system using Convolutional Neural Networks and custom activation functions to improve accuracy of character classification.

### Introduction 
- Classification of the handwritten Devanagari characters using Convolutional Neural Networks .
- The classification of Devanagari character is considered much more complex when compared to any other widely spoken languages.
- The language consists of 36 consonants .
- We used the data available in UCI repository which has 92K images of 32x32 pixel of each character.

### Problem 
- Now as this complex language has different writing styles, the recognition of character becomes much more difficult to tackle by conventional character recognition - techniques.
- The gradient learning problem occurs when the gradients computed during backpropagation are smaller than 1.
- In our approach we want tackle this problem and provide some solutions for better improvement of learning.

### Challenges
- The language has characters which have many curves and simple dots which has meaning. These features change the entire word and its context. 
- The kernel convolutions must be able to learn if the changes are small. For this problem, the Activation of neuron's plays a key role.
- The Most commonly  used Activation functions like Sigmoid, ReLU has gradient learning problems when the inputs are too small or when an activation has "–ve" effect are not considered.

### Approaches To Overcome the Challenges
- To overcome the challenge of gradient learning process. we focused on activation functions which can range differently for various inputs.
- Our approach is to customize the activation functions which can range well when the gradient is calculated.
- For example, if a convolution which has large value after max pooling, and it doesn't contribute to the right prediction ,the Activation should not be only zero. But  the neuron should also have "–ve" impact on it.

### Conclusion
We proposed a neural network model for the Devanagari Character Recognition. We trained a CNN classification model using customized activation functions viz. param_sigmoid, relu_moid and param_tanh on the DHCD dataset to achieve the accuracy of 96.07%. 


### References
[1] Mohite, A., & Shelke, S. (2018). Handwritten Devanagari Character Recognition using Convolutional Neural Network. Retrieved 2020, from https://ieeexplore.ieee.org/document/9057991/authors#authors  

[2] Bhaskar, S., Lavassar, N., & Green, S. (2010). Implementing Optical Character Recognition on the Android Operating System for Business Cards. Retrieved 2020, from https://www.semanticscholar.org/paper/Implementing-Optical-Character-Recognition-on-the-Bhaskar-Lavassar/1bf3c55d17214452970497a0915ee945464d5742  

[3] S. Acharya, A. K. Pant and P. K. Gyawali, "Deep learning based large scale handwritten Devanagari character recognition," 2015 9th International Conference on Software, Knowledge, Information Management and Applications (SKIMA), Kathmandu, 2015, pp. 1- 6. doi: 10.1109/SKIMA.2015.7400041 

[4] Joshi, R., Goel, P., & Joshi, R. (2020, January 19). Deep Learning for Hindi Text Classification: A Comparison. Retrieved 2020, from https://arxiv.org/abs/2001.10340 

[5] R. M. K. Sinha, “A journey from Indian scripts processing to Indian language processing,” IEEE Ann. Hist. Comput., vol. 31, no. 1, pp. 8–31, Jan./Mar. 2009. 

[6] J. Schmidhuber, "Deep Learning in Neural Networks: An Overview," Neural Networks, vol. 61, pp. 85-117, Jan. 2015. [Online]. Available https://arxiv.org/abs/1404.7828.Deep Learning Based Real Time Devanagari Character Recognition 62 

[7] A. Ray, A. Chandawala and S. Chaudhury, "Character Recognition Using Conditional Random Field Based Recognition Engine," 2013 12th International Conference on Document Analysis and Recognition, Washington, DC, 2013, pp. 18-22. doi: 10.1109/ICDAR.2013.13 

[8] V. Ganapathy and C. C. H. Lean, "Optical Character Recognition Program for Images of Printed Text using a Neural Network," 2006 IEEE International Conference on Industrial Technology, Mumbai, 2006, pp. 1171-1176. doi: 10.1109/ICIT.2006.372591 

[9] V. Bansal and R. M. K. Sinha, “Segmentation of touching and fused Devanagari characters,” Pattern Recognit., vol. 35, pp. 875–893, 2002. 

[10] H. Zhao, Y. Hu and J. Zhang, "Character Recognition via a Compact Convolutional Neural Network," 2017 International Conference on Digital Image Computing: Techniques and Applications (DICTA), Sydney, NSW, 2017, pp. 1-6.  doi: 10.1109/DICTA.2017.8227414 
