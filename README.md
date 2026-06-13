## AI Medical Diagnosis Assistant
It is a chatbot designed to help users understand potential health conditions based on symptoms they provide.It offers preliminary guidance and health-related information, helping users make informed decisions about seeking medical care.
The system uses Natural Language Processing (NLP) and machine learning techniques to analyze user input and suggest possible medical conditions, while encouraging consultation with qualified healthcare 

## Technologies Used
* Python
* Machine Learning
* Natural Language Processing (NLP)
* Flask
* Pandas
* Deepseek API


## Features
* Symptom-based analysis that suggests possible conditions from user input.
* AI-powered natural language understanding for smooth, conversational interaction.
* Preliminary diagnosis support that provides health insights and next-step guidance.
* Web-based chatbot interface built with Flask for easy access and use.

* ## The Process
## The Backend Methodology
The system is built using a Retrieval-Augmented Generation (RAG) approach. A medical encyclopedia PDF was used as the core knowledge source, which was first extracted and split into smaller text chunks for better processing. These chunks were then converted into vector embeddings using an embedding model to capture their semantic meaning.

The embeddings were stored in a Pinecone vector database, forming a searchable knowledge base. When a user asks a question, the system retrieves the most relevant chunks from this database based on semantic similarity. Finally, the DeepSeek AI API converts the retrieved vector-based information into clear, human-readable responses that the user can understand through the chatbot interface.
