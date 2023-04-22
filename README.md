# UCVME-Implementation
Here I am going to reproduce the results of an ML Article

## Source Article
The main resource is https://github.com/xmed-lab/UCVME.

## Author
Mohammad Javad Maheronnaghsh

## Goal
The goal is to reproduce the results of an article, and report the results and the way and details of doing that in this repository.
Thie name of the article is: "Semi-Supervised Deep Regression with Uncertainty Consistency and Variational Model Ensembling via Bayesian Neural Networks".

## Common Errors
### Proxy Error
Due to the use of proxies in Iran, when I wanted to clone from https://github.com/xmed-lab/UCVME.git, I faced a problem:
Unable to clone because of proxy.com.
To solve this problem, I entered "git config --global --unset http.proxy" in gitbash and this problem is resolved.
Now I can clone from the main repository.
### Picture Not Found Exception
This may happen  because we have forgotten to donwload and place the dataset in the correct place.
### CV2
To install CV2 package it is neccessary to install OpenCV in python (not cv2), because there is no module named "cv2" that is recognizable for Pycharm.


## Process
### Clone
First of all, I have cloned from the main repository (https://github.com/xmed-lab/UCVME.git) in Pycharm (locally).
### Dataset Download
In this step, I have downloaded the dataset from https://susanqq.github.io/UTKFace/.
In this webpage, I have downloaded the "Aligned&Cropped Faces" zip file, then etracted it and copied and pasted the images into the UTKFace directory in the cloned ptoject.
Note that if we forget to download the dataset, we are going to face an exception (Not Found Exception).
### Intalling Libraries
I opened the "__init__.py" file and installed the neccessary (and not-installed) libraries to my directory.
This task can be done in 3 ways:
-- Use another Configuration in Pycharm that satisfies the needed libraries.
-- Intall the libraries by entering the proper command in command line.
-- Simply Click "Alt+Enter" on the red part of the code (which is the not-satisfied library) and click on "Install Package".

It is also neccessary to add the libraries to "requirements.txt" file.
![image](https://user-images.githubusercontent.com/77095635/233777521-fd60f650-dcf0-497a-8c34-d9648ef6aba8.png)

### Training
We can start training process by writing this command (python3 ucvme_age.py --output='out') in the terminal.
When we start trainig, first resnet starts to download:
![image](https://user-images.githubusercontent.com/77095635/233778617-d2b76641-b9a9-46e0-88f0-1a56a79ea3ed.png)
Then the images are trained, etc. as wee can see in the below screenshot.
![image](https://user-images.githubusercontent.com/77095635/233790738-9550068b-e1f7-49f4-9e2d-a87837ad7f73.png)

### Testing
After entering this (python3 ucvme_age.py --output='out' --test_only) in the terminal, we can see the below picture that the pictures are on the test:
![image](https://user-images.githubusercontent.com/77095635/233790906-6da84a76-7306-455c-854b-35a3e2f3b651.png)



## Details
- I have done these processes in Windows 10. It can be done in Linux, too.


## Improvements and Suggestions
- I suggest to place the dataset in the main github repository, so we can train and test the model easily.
- I suggest to use another function instead of "imread" because Pycharm preferes to use the other methods.
- I suggest to create different repositores so we can update and add some comments to the github repository. In the current version, we only have a main branch that is not good for improving big projects and codes.
