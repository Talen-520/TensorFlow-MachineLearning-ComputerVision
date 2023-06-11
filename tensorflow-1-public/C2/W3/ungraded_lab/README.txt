In assignment, overfitting occured in vaildation set, to deal with this

Another useful tool to explore at this point is the Dropout. 

The idea behind it is to remove a random number of neurons in your neural network. This works very well for two reasons: The first is that neighboring neurons often end up with similar weights, which can lead to overfitting, so dropping some out at random can remove this. The second is that often a neuron can over-weigh the input from a neuron in the previous layer, and can over specialize as a result. Thus, dropping out can break the neural network out of this potential bad habit! 

Check out Andrew's terrific video explaining dropouts here: 
https://www.youtube.com/watch?v=ARq74QuavAo


在大的神经网络API model上使用dropout 有可能避免过度拟合

You saw Transfer Learning, and how you can take an existing model, freeze many of its layers to prevent them being retrained, and effectively 'remember' the convolutions it was trained on to fit images. 

You then added your own DNN underneath this so that you could retrain on your images using the convolutions from the other model. 

You learned about regularization using dropout to make your network more efficient in preventing over-specialization and thus overfitting.