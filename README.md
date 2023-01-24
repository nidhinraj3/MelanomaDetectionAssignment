### <font color='Navy' size='4'><b>Melanoma Detection using CNN</b></font>
<font color='Green' size='3'><u><b>Problem Statement</b></u></font>
<br />
To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.


## Table of Contents
* [Keras Tensorflow](#general-information)
* [Important Utilities Used](#technologies-used)
* [Conclusions](#conclusions)


<!-- You can include any other section that is pertinent to your problem -->

## Keras Tensorflow
- Keras is a deep learning API written in Python, running on top of the machine learning platform TensorFlow. It was developed with a focus on enabling fast experimentation.
- We can run Keras on TPU or on large clusters of GPUs, and you can export your Keras models to run in the browser or on a mobile device.
- Keras is used in this assignment to solve the Image Classification challenge

## Important Utilities Used
- tf.keras.utils.image_dataset_from_directory utility heps to load data from disk efficiently
` Params:
   - directory - directory to load data from
   - validation_split - Optional float between 0 and 1, fraction of data to reserve for validation. 
   - subset - "Training" means only training dataset is returned
   - seed - 	Optional random seed for shuffling and transformations.
   - image_size - Size to resize images to after they are read from disk
   - batch_size - Size of the batches of data `
- Keras Rescaling
- Optimizer based on Adams Algorithm
- Augmentor Library to generate images
- Sparse Categorical Crossentropy Loss function
## Conclusions
- Without Applying Dropout & Data Augmentation data is overfitting
- After augmentation and dropout is applied overfitting is solved but accuracy is reduced
- Once class imbalance is fixed then model was able to predict with high accuracy on validation dataset
