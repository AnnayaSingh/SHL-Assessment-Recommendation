# SHL Assessment Recommendation System

This project implements a semantic search based recommendation engine to match hiring queries with relevant SHL assessments.

## Approach
- Scraped SHL assessment catalogue
- Generated embeddings using Sentence Transformers
- Used cosine similarity for semantic matching
- Exposed recommendations via FastAPI

## Files
- SHL_Assignment.ipynb : Main notebook
- final_predictions.csv : Recommendation output
- shl_assessments.csv : Scraped dataset

## Tech Stack
- Python
- Sentence-Transformers
- FastAPI
- Pandas
## API Endpoints

- GET /health  
Returns service status.

- POST /recommend  
Request:
{
  "query": "Looking for a Java developer",
  "top_k": 5
}

Returns top-k recommended SHL assessment URLs.
