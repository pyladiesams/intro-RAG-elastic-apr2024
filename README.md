
# An introduction to RAG with Elastic
### Presentation: [Introduction to RAG](workshop/Introduction_to_RAG.pdf)

## Workshop description
During the workshop you will learn what is Retrieval Augmented Generation, how it can increase trustability of LLM models and how to set up a RAG pipeline using Elastic.

## Requirements

Python version: >=3.8.5


## Usage
* Clone the repository
* Start Visual Studio Code and navigate to the solutions folder
* Launch Jupyter App `jupyter notebook`

## Notebooks

### Question answering

In the [`question-answering.ipynb`](solutions/question-answering.ipynb) notebook you'll learn how to:

- Retrieve sample workplace documents from a given URL.
- Set up an Elasticsearch client.
- Chunk documents into 800-character passages with an overlap of 400 characters using the `CharacterTextSplitter` from `langchain`.
- Use `OpenAIEmbeddings` from `langchain` to create embeddings for the content.
- Retrieve embeddings for the chunked passages using OpenAI.
- Persist the passage documents along with their embeddings into Elasticsearch.
- Set up a question-answering system using `OpenAI` and `ElasticKnnSearch` from `langchain` to retrieve answers along with their source documents.

### Chatbot

In the [`chatbot.ipynb`](solutions/chatbot.ipynb) notebook you'll learn how to:

- Retrieve sample workplace documents from a given URL.
- Set up an Elasticsearch client.
- Chunk documents into 800-character passages with an overlap of 400 characters using the `CharacterTextSplitter` from `langchain`.
- Use `OpenAIEmbeddings` from `langchain` to create embeddings for the content.
- Retrieve embeddings for the chunked passages using OpenAI.
- Run hybrid search in Elasticsearch to find documents that answers asked questions.
- Maintain conversational memory for follow-up questions.



## Video record
Re-watch [this YouTube stream](https://www.youtube.com/live/TQdK9OsfHQk)

## Credits
This workshop was set up by @pyladiesams and @ahavrius
