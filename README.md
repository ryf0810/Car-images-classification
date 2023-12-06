# car-images-classification-project

Please rename the archive folder after untar to data

- Usage:
  after untar the data obtained online and rename to data, run create_label_file first, then run the model_parallel.py in terminal. You can adjust the batch size/learning rate/... to test

- data can be found here: https://www.kaggle.com/datasets/gogotchuri/myautogecardetails
  - suggest to only contain first 1000 to 2000 images folder and play around the adjustable parameters
  - running on whole dataset 18G will take roughly 4-5hours per epoch on 1 CPU, 1 hour per epoch on 1 GPU
- create_label_file.py will create a csv file for dataloader under ./data
- model.py 3 convolutional layer with 2 fully connected layer structure, and train the model using cross entropy loss
- model_parallel.py run the model on 4 CPUs


# Network Structure
-  All convolutional layers and 1st fully connected layers are followed by a relu activation function, no relu function after pooling layer
<img width="991" alt="image" src="https://github.com/ryf0810/car-images-classification-project/assets/106381479/8cbbc174-32ae-4db7-b94c-5a7ee13bff60">
