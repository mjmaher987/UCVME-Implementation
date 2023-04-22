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


## Process
### Clone
First of all, I have cloned from the main repository (https://github.com/xmed-lab/UCVME.git) in Pycharm (locally).
## Intalling Libraries
I opened the "__init__.py" file and installed the neccessary (and not-installed) libraries to my directory.
![image](https://user-images.githubusercontent.com/77095635/233777521-fd60f650-dcf0-497a-8c34-d9648ef6aba8.png)

### Training
