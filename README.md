# Medical-Chatbot-Using-Llama2
An End to End Medical Chatbot Project Using Llama2, LangChain, Flask, Pinecone

## Pre-requisites
Tech Stack used in this project:
1. Python (Programming Language)
2. LangChain (Generative AI)
3. Flask (Web App Implementation)
4. Llama 2 (LLM)
5. Pinecone (VectorStore)

## Project Architecture
_**Back-end Architecture:**_
![image](https://github.com/Kowshik-407/Medical-Chatbot-Using-Llama2/assets/66817358/b974e992-0492-42f0-991c-a8f56eed209e)


_**Components:**_
1. PDF File (Medical Books): Loading the medical books as a DATA SOURCE to the LLM
2. Extract Data or Information from the PDF file
3. Creating the whole data into Text Chunks [Because, the GPT models have a limited Context Window - Using Llama 2 (Context Window - 4096 Tokens)]
4. Creating Embeddings for every chunk.
5. Implementing the Semantic Index (Word2Vec - King, Queen Clustering)
6. Creating Vector Database (Pinecone Vectorstore)

_**Front-end Architecture:**_
![image](https://github.com/Kowshik-407/Medical-Chatbot-Using-Llama2/assets/66817358/a9d9fcc5-a358-4529-bc37-cef7abd69cb4)

## Project Creation
**Process:**
  - Setting up the Development Environment in VSCode
  - Few experiments in Anaconda Notebook
  - Coverting the Anaconda Notebook code into Modular Code
  - Creation of WebAPI using Streamlit

**Execution:**
1. Download this ZIP file
2. Open Terminal in VSCode, then execute the below commands:
- Creation of Virtual Environment
```
conda create -p mcq_env python=3.8 -y
```
- Activate the environment
```
source activate ./mcq_env
```
3. Create a .env file and add the below line:
```
PINECONE_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
PINECONE_API_ENV = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
```
4. Setup the requirements
```
pip install -r requirements.txt
```
5. Download the Quantize Model
```
## Download the Llama 2 Model:
llama-2-7b-chat.ggmlv3.q4_0.bin

## From the following link:
https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML/tree/main
```
6. Execute the webapp in the terminal
```
python app.py
```
