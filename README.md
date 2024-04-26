# Enhancing Search Engine Relevance for Video Subtitles_T211080
The Subtitles Search Engine is a project aimed at enhancing the search relevance for video subtitles, with a focus on improving the accessibility of video content.
Developed during my internship at Innomatics Research Labs by [Sakshi Nandardhane (IN1240908)] and [Kushal Adhyaru ( IN1240715)], this project leverages natural language processing (NLP) and machine learning (ML) techniques to provide more accurate and relevant search results for users.

# Features
1. Keyword-Based and Semantic Search: The search engine supports both keyword-based and semantic search, allowing users to find subtitles based on exact keyword matches or by understanding the meaning and context of their queries.
2. Document Chunker: To handle large subtitle documents effectively, the project includes a document chunker that divides them into smaller, more manageable chunks.
3. Vectorization Techniques: Experimentation with Bag-of-Words (BOW), Term Frequency-Inverse Document Frequency (TFIDF), and BERT-based "SentenceTransformers" for generating text embeddings.
4. Cosine Similarity Calculation: The cosine similarity between the vectorized documents and user query embeddings is calculated to determine the relevance of search results.

# How It Works
1. Ingesting Documents:
The subtitle data is ingested and cleaned, removing timestamps and applying preprocessing steps.
Large documents are chunked into smaller sections to handle information loss and improve efficiency.
2. Vectorization:
Text documents are vectorized using various techniques, including BOW, TFIDF, and BERT-based embeddings.
3. Storing the embeddings using ChromaDB:
This involves creating a client and specifying a path and name of the vector database and uploading the vectors using collection.add()
4. Retrieving Documents:
User queries are preprocessed, and query embeddings are generated.
Cosine similarity scores between document embeddings and query embeddings are calculated to retrieve relevant documents.

# Screenshots
![Screenshot 2024-04-26 125446](https://github.com/SakshiYN/Enhancing-Search-Engine_T211080-Relevance-for-Video-Subtitles_/assets/122168058/b6f9f79c-c15b-452a-881f-8eb9822c2d82)

![Screenshot 2024-04-26 121346](https://github.com/SakshiYN/Enhancing-Search-Engine_T211080-Relevance-for-Video-Subtitles_/assets/122168058/e038498c-30c6-4eb9-9bc1-4284f90a8a0d)

![Screenshot 2024-04-26 125532](https://github.com/SakshiYN/Enhancing-Search-Engine_T211080-Relevance-for-Video-Subtitles_/assets/122168058/f9b6c98a-22c5-45f1-bc6c-b9cfc5183884)

