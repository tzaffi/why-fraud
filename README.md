# why-fraud 🕵

Example project investigating the modeling of riskiness of fraudulent transactions and interpreting the results of model evaluation.

This is based on Kaggle's [IEEE-CIS Fraud Detection](https://www.kaggle.com/c/ieee-fraud-detection) competition.

## Running locally

To run locally, the following neeed to be installed:

* `make`
* `awk`
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

#### Clean up everything, except the images which took so long to build!!!

`make clean` 

Note: this only works when the container is running. So you might need to do a `make up` before running this command

#### Clean up everything, INCLUDING the images:

`make wipeout`

### Where did all my Jupyter notebooks go?

Persistent volumes are created by Docker on the file system. For _Ubuntu_ the path is:

`/var/lib/docker/volumes/`

In particular, the **exploration** notebooks are under `/var/lib/docker/volumes/why-fraud_exploration/_data/
` 




