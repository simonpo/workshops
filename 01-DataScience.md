# Workshop 1: Data Science Hands On

## Introduction

Before the team can begin working on Data Science topics, everyone needs to have a development environment set up with approriate tools. This workshop will get you ready to begin developing, and includes hands-on experience with the following elements:

* Signing in to Azure
* Connecting to an Ubuntu DSVM
* Modeling lifecycle using ML Studio and SDK
* Using Databricks cluster as a compute target

Take a look at these repos for additional information:

* [Azure ML SDK for Python Docs](https://docs.microsoft.com/en-us/python/api/overview/azure/ml/intro?view=azure-ml-py)
* [Jupyter notebooks](https://github.com/Azure/MachineLearningNotebooks)
* [Samples for AI](https://github.com/Microsoft/samples-for-ai)

## Signing in to Azure

Sign in to the [Azure portal](https://portal.azure.com) using your credentials.

## Connecting to an Azure Ubuntu DSVM

[Section 1.1](01.1-DSVM.md) explains how to connect to an Ubuntu Data Science Virtual Machine in Azure, and provides a brief introduction to Jupyterhub.

## Modeling lifecycle using Azure ML Python SDK and Azure Databricks

[Section 1.2](01.2-AMLwithDatabricks.md) explains how to set up Azure ML Python SDK in Azure Databricks, prepare data, build model, train and deploy.

## Using Ubuntu DSVM as a compute target

A compute target is the resource that runs your training script or hosts your model when it's deployed as a web service. Azure ML Python SDk can create and manage a new compute target, or attach the existing one to the ML workspace. Data Science Virtual Machine (DSVM) running Ubuntu can be compute target, and that supports GPU acceleration, Automated hyperparameter tuning, Automated model selection, and can be used in pipelines.  

Review [DSVM as Computer Target Steps by Step instruction](https://docs.microsoft.com/en-us/azure/machine-learning/service/how-to-set-up-training-targets#dsvm). This is [Jupyter Notebook](https://github.com/Azure/MachineLearningNotebooks/blob/master/01.getting-started/04.train-on-remote-vm/04.train-on-remote-vm.ipynb) that demonstrates training on a Data Science Virtual Machine.