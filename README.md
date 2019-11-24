# why-fraud 🕵

Example project investigating modeling of riskiness of fraudulent transactions
and interpreting the results of the model evaluation

This is based off Kaggle's [IEEE-CIS Fraud Detection](https://www.kaggle.com/c/ieee-fraud-detection) competition.

## Running locally

To run locally, the following neeed to be installed:

* `make`
* the `docker` family of applications

### Available commands

`make help` 

### Build all services

`make build`

### Start all services in interactive mode:

`make iup`

### Explore the data in a Jupyter notebook:

1. Run `make iup` and note the authorization token printed in the logs
2. Navigate to http://localhost:8899
3. Paste the autorization token that you copied in step 1 into the text box that appears



