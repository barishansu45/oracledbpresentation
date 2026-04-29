# Oracle 23ai AI Vector Search Demo

This project was developed for the **Modern Large Scale Systems** course at **Yaşar University**. It demonstrates the native vector search capabilities of the modern Oracle 23ai Database through an interactive Streamlit web interface.

## 🚀 Features
- **Oracle 23ai Vector Search:** Performs semantic search directly within the database using the new `VECTOR` data type and `VECTOR_DISTANCE` function.
- **Docker Integration:** The database runs in an isolated local environment using the official Oracle 23ai Free Docker container.
- **AI Embedding:** Utilizes the `all-MiniLM-L6-v2` model from Hugging Face (`sentence-transformers`) to convert text data into 384-dimensional vector embeddings.
- **Interactive UI:** Built with Streamlit for a seamless and responsive user experience.

## 🛠️ Prerequisites
- [Docker Desktop](https://www.docker.com/products/docker-desktop/)
- Python 3.8+

## 📦 Installation & Setup

**1. Start the Oracle 23ai Database via Docker:**
```bash
docker run -d --name oracle23ai -p 1521:1521 -e ORACLE_PWD=Oracle_123_ [container-registry.oracle.com/database/free:latest](https://container-registry.oracle.com/database/free:latest)
