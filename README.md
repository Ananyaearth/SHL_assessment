# SHL Assessment Recommendation System

A Retrieval-Augmented Generation (RAG) pipeline for recommending SHL assessments, deployed as a FastAPI app on Render.com.

## Repository Structure

### Folders
- **`get_api_assessment-main/`**: FastAPI app files for API-based deployment on Render.com.
  - **Repo URL**: [https://github.com/Ananyaearth/get_api_assessment](https://github.com/Ananyaearth/get_api_assessment)
  - **Website URL**: [https://get-api-assessment.onrender.com](https://get-api-assessment.onrender.com)
  - **Example Usage** --> https://get-api-assessment.onrender.com/recommend?query=Java+developers
  - **`app.py`**: FastAPI script serving RAG responses via GET API.
  - **`requirements.txt`**: Dependencies (e.g., FastAPI, FAISS, Sentence Transformers).
  - **`shl_assessments_index.faiss`**: FAISS index for embedded assessment data.
  - **`shl_catalog_detailed.csv`**: Scraped SHL assessment dataset.
- **`new_SHL-main/`**: Streamlit app files for cloud-hosted web interface.
  - **Repo URL**: [https://github.com/Ananyaearth/SHL_assessment](https://github.com/Ananyaearth/SHL_assessment) (assuming this is the main repo hosting `new_SHL-main`)
  - **Website URL**: [https://newshl.streamlit.app/](https://newshl.streamlit.app/)
  - **`app.py`**: Streamlit script for interactive web-based querying.
  - **`requirements.txt`**: Dependencies (e.g., Streamlit, FAISS, Pandas).
  - **`shl_assessments_index.faiss`**: FAISS index for embedded assessment data.
  - **`shl_catalog_detailed.csv`**: Scraped SHL assessment dataset.

### Files
- **`Data_Acquistion.ipynb`**: Jupyter notebook with Selenium script to scrape SHL assessment data.
- **`experimentation.ipynb`**: Notebook for testing preprocessing, embedding, FAISS, and RAG development.
- **`README.md`**: Project overview and structure documentation.

## Overview
- Scraped SHL data using Selenium in `Data_Acquistion.ipynb`.
- Experimented with preprocessing, FAISS, and RAG using Google Gemini in `experimentation.ipynb`.
- Deployed a Streamlit web app via `new_SHL-main/` and finalized an API solution in `get_api_assessment-main/` on Render.com.

