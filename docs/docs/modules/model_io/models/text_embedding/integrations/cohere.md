# Cohere

Let's load the Cohere Embedding class.

<!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! Instead, edit the notebook w/the location & name as this file. -->


```python
from langchain.embeddings import CohereEmbeddings
```


```python
embeddings = CohereEmbeddings(cohere_api_key=cohere_api_key)
```


```python
text = "This is a test document."
```


```python
query_result = embeddings.embed_query(text)
```


```python
doc_result = embeddings.embed_documents([text])
```