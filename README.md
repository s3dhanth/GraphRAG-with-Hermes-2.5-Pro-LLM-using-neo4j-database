# GraphRag-for-Hermes-2.5-Pro-LLM-using-neo4j-database

This repository contains a Graph node implementation to extract the relations between text by using Cypher Language for enhanced Retrieval aungmented generation Q&A bot that leverages Hermes 2.5 pro and Graph Database with Docker Integration. The app allows users to interact with the Model and get responses based on their queries.

## DataSet

- Data: The Story of Amico’s Family

## Graph Data Store(Cypher Language)
- Converted document chunks into Cypher based graph node using LLaMA 3.1 Embedding (4096 vectors)
  ![graphph](https://github.com/user-attachments/assets/3de48bf6-3639-4ea7-b7eb-2eaa9937d50d)


- Integrated docker Container with port 7687:7687

![dockergraph](https://github.com/user-attachments/assets/25bcd99f-5adb-40cd-90af-e8211ed55e77)


## Installation

1. Clone the repository:

```sh
git clone https://github.com/your-username/rag_project.git
cd rag_project
Install the required dependencies:
sh
Copy code
pip install -r requirements.txt

# Create .env file & store the variables
- NEO4J_URL
- NEO4J_USERNAME
- NEO4J_PASSWORD
```

2. Docker setup for Neo4j
```sh
# To Integrate with Docker
cd GRAPHRAG-WITH-LLAMA-3.1
change (user/password)
docker-compose up --build

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.
```
- Enter your credentials to the Port specified
![image](https://github.com/user-attachments/assets/2defcf2a-0646-4430-8ca1-99108939bdcc)

## Model DEMO (LLaMA 3.1)
- GRAPH NODE 
![node](https://github.com/user-attachments/assets/86dac887-49a9-42fa-9aca-6c50f696fb82)
- 5 nearest Neighbor GraphNode based on querry (it will be converted to text and added onto the context window on final prompt)
![node_db](https://github.com/user-attachments/assets/a2673410-89bf-41a2-a7c1-c967d1d6dffa)
- querry & output
![output](https://github.com/user-attachments/assets/2af648b0-df62-4afe-b256-ff31c6dab098)


