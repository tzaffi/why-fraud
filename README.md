# why-fraud 🕵

Example project investigating the modeling of riskiness of fraudulent transactions and interpreting the results of model evaluation.

This is based on Kaggle's [IEEE-CIS Fraud Detection](https://www.kaggle.com/c/ieee-fraud-detection) competition.

## Running locally

To run locally, the following neeed to be installed:

* `make`
* the `docker` family of applications

### Available commands:

`make help` 

### Build all services:

`make build`

### Start all services in interactive mode:

`make iup`

### Explore the data in a Jupyter notebook:

1. Run `make iup` and note the authorization token printed in the logs
2. Navigate to http://localhost:8899
3. Paste the authorization token that you copied in step 1 into the text box that appears


### Cleaning up

`make clean`

1. docker rm *VARIOUS IMAGES*
2. docker rmi why-fraud-explore:latest

### Where did all my Jupyter notebooks go?

Persistent volumes are created by Docker on the file system. For _Ubuntu_ the path is:

`/var/lib/docker/volumes/`

In particular, the **exploration** notebooks are under `/var/lib/docker/volumes/why-fraud_exploration/_data/
` 




