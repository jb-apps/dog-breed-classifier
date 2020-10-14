# Dog-breed-classifier
Model that given an image of a dog, it will identify an estimate of the canine’s breed. If a human image is supplied, the code will identify the resembling dog breed.

# Data
Two datasets are provided [dog-dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip)(8351 images) and [human-dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/lfw.zip) (13233 images).

# Process
The project mainly consists of two parts, creating a CNN from scratch and transfer learning.

# Scratch CNN Architecture to detect dog breeds
12% accuracy after 30 epochs
![Image](https://github.com/jb-apps/dog-breed-classifier/blob/main/Scratch_CNN.png)

# Transfer learning Architecture to detect dog breeds
82% accuracy after only 5 epochs!
VGG16 was used and only the very last classification layer was trained, the reason behind it is because VGG16 is already able to detect dog features and our training data was very small.

# Future improvements
- Use a different network for transfer learning, resnet for example.
- Tweak VGG16 parameters (weight initialization, dropout, ).
