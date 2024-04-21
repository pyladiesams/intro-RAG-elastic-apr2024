
# An introduction to RAG with Elastic
### Presentation: [Introduction to RAG](workshop/Introduction_to_RAG.pdf)

## Workshop description
During the workshop you will learn what is Retrieval Augmented Generation, how it can increase trustability of LLM models and how to set up a RAG pipeline using Elastic.

## Requirements 🧰

For this workshop, you will need:

- Python 3.6 or later
- An Elastic deployment
  - We'll be using [Elastic Cloud](https://www.elastic.co/guide/en/cloud/current/ec-getting-started.html) for this example (available with a [free trial](https://cloud.elastic.co/registration?utm_source=github&utm_content=elasticsearch-labs-notebook))
- OpenAI account


## Usage
* Clone the repository
* Start your favorite IDE and navigate to the solutions folder
* Run `pip install -r requirements.txt`
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
