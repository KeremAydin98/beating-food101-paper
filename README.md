# beating-food101-paper
Beating an image classification paper by utilizing the fine tuning method

Fine tuning was used to pass the validation accuracy of Food101 paper. Even though only 50% of the data was used, the validation accuracy of 72.37% has been achieved. The validation accuracy is 50.76% in the paper.  

I have used mixed precision to speed up the process. Tensorflow's decription for the mixed precision is: "Mixed precision is the use of both 16-bit and 32-bit floating-point types in a model during training to make it run faster and use less memory". Therefore tensorflow transforms some of the 32-bit points to the 16-bit points so that the training can be done faster. However the GPU you are using, must have more than 7.0 compute capability score. I have used Google Colab's Tesla T4 GPU to implement this. The other free GPUs don't have enough compute capability score to use mixed precision, so try to restart the kernel until you get Tesla T4 if you want to use mixed precision in your training. 

### Libraries that have been used:
* tensorflow
* tensorflow_datasets
* matplotlib.pyplot

The paper can be accessed through this link:

https://data.vision.ee.ethz.ch/cvl/datasets_extra/food-101/static/bossard_eccv14_food-101.pdf
