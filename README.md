# LangChain with Neo4j Graph Database

A simple project demonstrating how to connect **LangChain** with **Neo4j Graph Database** to perform natural language question answering using **GraphCypherQAChain**.

## 🚀 Features

- Connect LangChain with Neo4j
- Store graph data in Neo4j
- Generate Cypher queries from natural language
- Execute Cypher queries on the graph database
- Generate human-readable answers using an LLM
- Supports Groq (Llama 3)

---

## 🛠️ Tech Stack

- Python
- LangChain
- Neo4j
- GraphCypherQAChain
- Groq (Llama 3)
- Cypher Query Language

---

## 📂 Project Structure

```
.
├── 1-Q&A With GraphDb.ipynb
├── requirements.txt
├── .env
├── .gitignore
└── README.md
```

---

## 🔑 Environment Variables

Create a `.env` file.

```env
GROQ_API_KEY=your_groq_api_key

NEO4J_URI=bolt://localhost:7687
NEO4J_USERNAME=neo4j
NEO4J_PASSWORD=your_password
```

---

## ▶️ Run Project

Open the notebook:

```
1-Q&A With GraphDb.ipynb
```

Run all cells sequentially.

---

## ⚙️ Workflow

```
User Question
      │
      ▼
LangChain
      │
      ▼
GraphCypherQAChain
      │
      ▼
Generate Cypher Query
      │
      ▼
Neo4j Graph Database
      │
      ▼
Execute Query
      │
      ▼
Query Result
      │
      ▼
LLM Generates Final Answer
```

---

## 🧠 Example Questions

- Who is the CEO of Tesla?
- Which company does Elon Musk lead?
- Show all companies.
- List all people.
- Who works at Microsoft?
- Find employees of Google.

---

## 📝 Example Cypher Query

```cypher
MATCH (p:Person)-[:CEO_OF]->(c:Company)
RETURN p.name, c.name
```

---

## 📚 Concepts Covered

- Graph Databases
- Neo4j
- Nodes & Relationships
- Labels & Properties
- Cypher Query Language
- LangChain
- GraphCypherQAChain
- LLM Integration
- Natural Language to Cypher Conversion

---

## 🎯 Learning Outcomes

By completing this project, you will learn:

- Neo4j graph database fundamentals
- Writing and understanding Cypher queries
- Integrating Neo4j with LangChain
- Converting natural language into Cypher queries
- Building graph-based question-answering applications

---

## ⭐ If you found this project helpful, consider giving it a star!
