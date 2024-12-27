# Semantic Spotter Project ~ Kiran Dalmiya

Semantic Spotter is a Retrieval-Augmented Generation (RAG) application designed to efficiently search and answer questions from insurance policy documents. This project leverages LlamaIndex and GPT-3.5-turbo for its functionality.

## Table of Contents
- [General Info](#general-information)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Deployment](#deployment)
- [Conclusions](#conclusions)
- [Acknowledgements](#acknowledgements)
- [Contact](#contact)



## general-information

 **Problem Statement -

  We are provided with a Insurance policy documents. Our goal here is to build a simple RAG application on the provided policy pdf document.

  * **Solution Strategy -** Build a POC which should solve the following requirements:

    * Users would get responses from the Insurance policy document.
    * If they want to refer to the original page from which the bot is responding, the bot should provide a citation as well.

  * **Goal -** Solving the above two requirements well in the POC would ensure that the accuracy of the overall model is good and therefore further improvisations and customizations make sense.

  * **Data Used -** Insurance Policy document in pdf formate stored in a single folder

  * **Tools used -** LlamaIndex has been used due to its powerful query engine, fast data processing using data loaders and directory readers as well as easier and faster implementation using fewer lines of code.

The main goal of this project was to build a smart system that can search through documents and give clear, helpful answers to questions.

 It combines two powerful tools:
   * 	**LlamaIndex** (to search and find relevant information in documents)
   * 	**GPT-3.5-turbo openai model** (to improve the answers and make them more user-friendly).


This system was designed to answer questions specifically related to insurance policy documents.


## Prerequisites

Before you begin, ensure you have met the following requirements:

- Google Colab account
- Python 3.x installed
- Required libraries:
  - `llama_index`
  - `openai`
  -  pandas


## Installation

Install the required libraries:

!pip install llama_index openai
!pip install -U -qq openai llama-index 
!pip install llama-index-core llama-index-readers-file 
!pip install llama-index-llms-openai llama-index-embeddings-openai

If you are using additional libraries, ensure they are installed as well.


## Usage

Open your Google Colab notebook where the Semantic Spotter program is implemented.

Load your documents (e.g., insurance policies) into the environment. 
Ensure they are in a format that your program can read (e.g., PDF, text).

Run the following code snippets in the appropriate order:

	# Import necessary libraries
	from llama_index import ...  # Your specific imports

	# Initialize your model
	model = ...  # Initialization code

	# Load your documents
	documents = ...  # Code to load your documents

	# Process the documents
	index = ...  # Create an index or embeddings

	# Run all the function in the notebook and query the model
	response = model.query("Your question here")
	print(response)

	# Run interactive_conversation_with_evaluation() for the final response 
	interactive_conversation_with_evaluation()


Replace "Your question here" with the question you want to ask based on the loaded documents.


## Deployment
To deploy this application:

Ensure that your Google Colab environment is set up and all dependencies are installed.

Share the Colab notebook with users or export it as a Python script for local execution.

If you plan to deploy it as a web application, consider using Flask or Streamlit to create a user-friendly interface.


## Conclusion
This project built an efficient query engine that quickly finds relevant information from documents and combines it with the conversational power of GPT-3.5-turbo with Llamaindex framework. It not only retrieves useful information but also improves the responses and adapts based on user feedback. The system can be further developed and applied to other areas like law, education, or finance, making it versatile beyond just insurance.

## Acknowledgements
- This project was inspired by live session of upGrad on Llamaindex and Semantic Spotter Project
- UpGrad tutorials on Llamaindex on the learning platform

## Contact
Created by [@kirandalmiya]  (https://github.com/kirandalmiya)


