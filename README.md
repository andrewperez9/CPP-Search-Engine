# CPP Biology Department Faculty Search Engine

## Description
This project is a full-stack search engine that indexes faculty pages from the Cal Poly Pomona Biology Department so that students can easily find faculty based on bioinformatics or biology-related keywords. It uses web scraping, TF-IDF vectorization, cosine similarity, and Flask APIs.

## Features
- Crawls and scrapes faculty web pages
- Builds TF-IDF vectors from relevant content
- Stores documents in MongoDB
- Serves a Flask API for querying
- Simple front-end to search and view results
- Uses NLTK for text processing and lemmatization

## Presentation
https://docs.google.com/presentation/d/1wwemX59ivfNctmGTFhGdr9RyHixwHhvYjShvPMSAhFs/edit?usp=sharing

## Requirements
- Python 3.7+
- MongoDB (running locally on port 27017)

## Getting Started

1. Clone repository

```git clone https://github.com/andrewperez9/CPP-Search-Engine.git```

2. Install dependencies

**First time build only**:

```
python 
import nltk 
nltk.download('punkt') 
nltk.download('wordnet') 
nltk.download('omw-1.4')
```

```pip install -r requirements.txt```

3. Start MongoDB

```brew services start mongodb-community@X.0```

4. Run Search Engine

```
cd SearchEngine
python crawler.py
python transformation.py
python information_retrieval.py
``` 
5. View in browser

Open http://127.0.0.1:5500/WebApp/index.html

## To Stop

CTRL+C \
```brew services stop mongodb-community@6.0```

