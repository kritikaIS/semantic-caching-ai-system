
# Semantic Caching System for AI Applications

## Overview
This project implements a semantic caching system that improves AI query processing efficiency by caching semantically similar queries.

## Features
- Semantic Search using Sentence Transformers
- Vector Search using FAISS
- Semantic Query Cache
- FastAPI REST API

## API Endpoints

POST /query  
GET /cache/stats  
DELETE /cache

## Run the API

Install dependencies:

```
pip install -r requirements.txt
```

Run server:

```
uvicorn app:app --reload
```

Open API docs:

```
http://localhost:8000/docs
```

## Demo

Example semantic caching workflow:

Query → Embedding → Cache Check → FAISS Search → Store in Cache

## Tech Stack
- Python
- FastAPI
- Sentence Transformers
- FAISS


