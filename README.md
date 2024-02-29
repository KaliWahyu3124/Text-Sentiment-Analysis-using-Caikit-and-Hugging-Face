# Text Sentiment Analysis using Caikit and Hugging Face

## Author: Unknown

## Mentee:
- Name: Wahyu Cahyono.P
- Program: IBM Advanced AI

## Tujuan:
- Melakukan text sentiment analysis. Mendetaksi apakah text tersebut terklasifikasi positif atau negatif

## Note: Semua file yang diunggah harus dibuat didalam satu direktori yang sama, text-sentiment

## Libraries Uses:
- virtualenv
- typing
- caikit, caikit.core, caikit.core.data_model
- .classification
- os
- transformers
- text_sentiment.data_model.classification
- scipy
- torch
- requirements.txt
- sys
- alog
- caikit.runtime

## Modules Uses:
- List
- DataObjectBase
- dataobject
- ClassificationPrediction, ClassInfo, TextInput
- HuggingFaceSentimentModule
- pipeline
- ModuleBase, ModuleLoader, ModuleSaver, TaskBase, module, task
- grpc_server
- ServicePackageFactory
- TextInput

## Directory Structurer:
- text-sentiment/                     # top-level package directory
- start_runtime.py                # a wrapper to start the Caikit runtime as a gRPC server. The runtime will load the model at startup
- client.py                       # client which calls the Caikit runtime to perform inference on the model it is serving to perform text sentiment analysis
- requirements.txt                # specifies library dependencies
- models/                         # a directory that contains the Caikit metadata of the model and any artifacts required to run the model
- text_sentiment/config.yml   # metadata that defines the Caikit text sentiment model
- text_sentiment/                 # a directory that defines Caikit module(s) that can include algorithm(s) implementation that can train/run an AI model
- config.yml                  # configuration for the module and model input and output
- __init__.py                 # makes the data_model and runtime_model packages visible
- data_model/                 # a directory that contains the data format of the Caikit module
- classification.py       # data class that represents the AI model attributes in code
- __init__.py             # makes the data model class visible in the project
- runtime_model/              # a directory that contains the Caikit module of the model
- hf_module.py            # a class that bootstraps the AI model in Caikit so it can be served and used (infer/train)
- __init__.py             # makes the module class visible in the project

## Complete the following tasks to configure the Caikit runtime and the AI model, and then test them from a client application:
- Create the project
- Create the data model specification
- Create the model wrapper
- Include the module and package dependencies
- Start the Caikit runtime
- Test the sentiment analysis
