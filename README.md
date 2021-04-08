# Resize the frame
The experiments were conducted without face alignment and face cropping to avoid a potential error source. In the experiments, frames were resized to a resolution of $224 \times 224$ pixels.

# Augmenting data by a sliding window
We augment the training data by extracting fixed-length video segments (sequences of consecutive frames) from each original video by overlapping sliding windows of size $N$ with a step size of 1. By intercepting the fixed-length video clip, which is the frame sequences of the same number $N$, training samples could be fed into the network in batches. 

As a smaller $N$ will lead to a loss of long-term dependence information and a larger $N$ will reduce the number of sequences, meanwhile, smaller $N$ bring about larger number of training samples to avoid overtraining and larger $N$ contains more information. We experimented with several combinations to find the appropriate value for $N$. 

# Flipping and Rotation
Mirror flipping or rotating image is a common method for data augmentation of image samples. We also applied flipping and rotation methods in the experiments to see how it improves the recognition results. 




