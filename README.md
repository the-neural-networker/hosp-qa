# hosp-qa
Hospital QA is a chatbot designed for querying and answering questions related to hospital systems. Built using open-source Large Language Models (LLMs) and Retrieval-Augmented Generation (RAG), it leverages a Neo4j database to store and query hospital system data.

This is project I built following https://realpython.com/build-llm-rag-chatbot-with-langchain to help me better understand how Retrieval Augmented Generation and LangChain work.
# To run:

## 1. Clone the Repository

```python
git clone https://github.com/the-neural-networker/hosp-qa.git
cd hosp-qa
```

## 2. Set Up Environment Variables

Create a file named `.env` in the root directory of the project and paste the contents of `.env-example` and fill the following environment variables according to your credentials appropriately:

```
OPENAI_API_KEY=your_openai_api_key

NEO4J_URI=your_neo4j_uri
NEO4J_USERNAME=your_neo4j_username
NEO4J_PASSWORD=your_neo4j_password
```

## 3. Build and Run the Application
Use Docker Compose to build and start the application:

```zsh
docker-compose up --build
```

## 4. Access the Application
Once the application is up and running, you can access the following services:

- Flask API: Accessible at http://localhost:8000
- Streamlit Frontend: Accessible at http://localhost:8501