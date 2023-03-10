
## Project Overview.  [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/) [![CircleCI](https://dl.circleci.com/status-badge/img/gh/antonnifo/psychic-barnacle/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/antonnifo/psychic-barnacle/tree/main)

In this project, you will apply the skills you have acquired in this course to operationalize a Machine Learning Microservice API. 

You are given a pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. You can read more about the data, which was initially taken from Kaggle, on [the data source site](https://www.kaggle.com/c/boston-housing). This project tests your ability to operationalize a Python flask app—in a provided file, `app.py`—that serves out predictions (inference) about housing prices through API calls. This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.


---

## Setup the Environment

* Create a virtualenv with Python 3.7 and activate it. Refer to this link for help on specifying the Python version in the virtualenv. 
```bash
python3 -m pip install --user virtualenv
# You should have Python 3.7 available in your host. 
# Check the Python path using `which python3`
# Use a command similar to this one:
python3 -m virtualenv --python=<path-to-Python3.7> .devops
source .devops/bin/activate
```
* Run `make install` to install the necessary dependencies

### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`

### Kubernetes Steps

* Setup and Configure Docker locally
* Setup and Configure Kubernetes locally
* Create Flask app in Container
* Run via kubectl. 

### Files in Repository
1. **run_docker.sh** - Files to build and run docker image  
 2. **upload_docker.sh** - Files to upload images to docker hub
 3. **run_kubernetes.sh** - Files to deploy to kubernetes
 4. **Makefile** - Files to build application
 5. **app.py** - Application file
 6. **requirements.txt** - Python dependencies to run the app
 7. **output_txt_files/docker_out.txt** - log output from Docker prediction
 8. **output_txt_files/kubernetes_out.txt** - log output from Kubernetes-mediated prediction
 9. **model_data/** - Folder for Application Models
 10. **.circleci/** - Folder for Circleci Config File

