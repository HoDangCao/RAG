# Retrieval-Augmented Generation (RAG)

RAG is a type of architecture used in NLP, especially for tasks that involve generating text or answering questions based on a knowledge base.

---

## I. Purpose of Project

Create RAG application for question answering over a document. These include extracting information, retrieving the relevant context, and utilizing this context to generate accurate results.

<img src="https://miro.medium.com/v2/resize:fit:1100/format:webp/0*hikPIs0EQ1CJ4qrz" alt="My Image" width="600">

Typical RAG Application

Step 1: extract information from this document.

Step 2: break the document into smaller chunks, to fit into LLM context windows.

Step 3: two strategies to save documents for future retrieval:
- store the text as-is for keyword based retrieval.
- convert text into vector embeddings, for more efficient retrieval.

Step 4: save this to a relevant database.

Step 5: obtain relevant chunks based on user inputs.

Step 6: incorporate relevant document chunks as part of LLM context, for generating the output.

`Note:` 
- Steps 1 - 4 are referred to as the indexing pipeline, wherein documents are indexed in a database offline, prior to user interactions. 
- Steps 5 - 6 happen in real-time as the user is querying the application.

## Implementation
- Chunking Data: Fixed Size Chunk
- Retrieval Methods
  - Keyword Based Retrieval
  - Vector Embeddings
- Augmented Generation
- Evaluation
