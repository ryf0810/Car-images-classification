# car-images-classification-project

Please rename the archive folder after untar to data

- data.tar.gz contains only first 2000 image folders, whole dataset can be found here: https://www.kaggle.com/datasets/gogotchuri/myautogecardetails
- create_label_file.py will create a csv file for dataloader under ./data
- model.py 3 convolutional layer with 2 fully connected layer structure, and train the model using cross entropy loss
- model_parallel.py run the model on 4 CPUs

Usage:
  after untar the file and rename to data, run create_label_file first, then run the model_parallel.py in terminal. You can adjust the batch size/learning rate/... to test


# Network Structure - each layer followed by a relu activation function
<img width="991" alt="image" src="https://github.com/ryf0810/car-images-classification-project/assets/106381479/8cbbc174-32ae-4db7-b94c-5a7ee13bff60">
