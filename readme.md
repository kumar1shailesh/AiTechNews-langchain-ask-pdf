# Langchain Ask PDF (Tutorial)

>You may find the step-by-step video tutorial to build this application [on Youtube AiTechNews](https://youtu.be/Ju-kuOX1ag8).

This is a Python application that allows you to load a PDF and ask questions about it using natural language. The application uses a LLM to generate a response about your PDF. The LLM will not answer questions unrelated to the document.

# Python require libraries

# langchain==0.0.316
# openai==0.28.1
# PyPDF2==3.0.1
# python-dotenv==1.0.0
# streamlit==1.18.1
# faiss-cpu==1.7.4
# altair<5

## Below code only for local
# pip install PyPDF2 python-dotenv streamlit faiss-cpu
# pip install langchain==0.0.316
# pip install openai==0.28.1
# pip install tiktoken

## To run the app 
streamlit run app.py

![image](https://github.com/kumar1shailesh/AiTechNews-langchain-ask-pdf/assets/111674342/a2a6367b-1f14-498f-b7b0-7d73141d1620)

## How it works

The application reads the PDF and splits the text into smaller chunks that can be then fed into a LLM. It uses OpenAI embeddings to create vector representations of the chunks. The application then finds the chunks that are semantically similar to the question that the user asked and feeds those chunks to the LLM to generate a response.

The application uses Streamlit to create the GUI and Langchain to deal with the LLM.


## Installation

To install the repository, please clone this repository and install the requirements:

```
pip install -r requirements.txt
```

You will also need to add your OpenAI API key to the `.env` file.

## Usage

To use the application, run the `main.py` file with the streamlit CLI (after having installed streamlit): 

```
streamlit run app.py
```


## Contributing

This repository is for educational purposes only and is not intended to receive further contributions. It is supposed to be used as support material for the YouTube tutorial that shows how to build the project.


