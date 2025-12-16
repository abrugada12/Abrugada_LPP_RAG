# A Beginner’s Guide to the Wizarding World

Harry Potter Retrieval-Augmented Generation (RAG) Assistant

**Project Description**

This project is a Retrieval-Augmented Generation (RAG) assistant designed to help new fans learn about the Harry Potter universe. The assistant answers questions using a curated collection of documents rather than relying only on a language model’s general knowledge.

The goal of this project is to make information about the Harry Potter series more accessible to beginners by providing clear, accurate, and engaging explanations supported by retrieved sources.

The assistant is deployed as an interactive Streamlit application.


**Domain Overview and Problem Statement**

The Harry Potter universe includes seven books, eight films, and a large number of characters, locations, and storylines. While the series is widely known, the amount of information can be overwhelming for someone who is just getting started.

Many people who are curious about the series may not know where to begin or which details are most important. This project addresses that problem by creating an assistant that focuses on foundational knowledge, such as major characters, key events, and central themes, while presenting information in a clear and beginner-friendly way.


**Architecture Overview (RAG Pipeline)**

This assistant is built using a Retrieval-Augmented Generation (RAG) architecture. The system combines document retrieval with a language model to generate responses grounded in the project’s document collection.

_Pipeline Overview:_
1. Document Collection: A curated set of documents related to the Harry Potter universe is collected and preprocessed.
2. Vector Database: The documents are embedded and stored in a DuckDB-based vector database. This allows the system to retrieve relevant passages based on a user’s query.
3. Retrieval Step: When a user submits a question, the system retrieves the most relevant document chunks from the vector database.
4. Generation Step: The retrieved content is passed to a language model, which generates a response grounded in those sources.
5. Streamlit Deployment: The assistant is deployed using Streamlit, allowing users to interact with the system through a simple web interface.

**Document Collection Summary**

The document collection includes a mix of formats to provide a well-rounded knowledge base:

_PDF Files:_

PDFs include structured content such as chapter summaries and character analyses. These documents provide clear overviews of plot points, character motivations, and key events. Their structured format makes them well-suited for chunking and retrieval.

_HTML Files:_

HTML files consist of web articles and guides that explore different aspects of the Harry Potter universe. These sources often use a conversational tone and include reflections, facts, and thematic discussions, making them accessible to newcomers while still offering meaningful insights.

_YouTube Transcripts:_

YouTube transcripts capture discussions, reviews, and analyses from fans and commentators. These sources introduce informal perspectives, rankings, and opinions, which add variety and depth to the assistant’s responses.

