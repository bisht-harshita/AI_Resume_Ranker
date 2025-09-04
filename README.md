# AI Resume Ranker

AI Resume Ranker is a web application that analyzes and scores resumes against job descriptions using ATS (Applicant Tracking System) criteria.  
It provides actionable suggestions to improve your resume's match with a given job description.

## Features
- Upload your resume (PDF) and job description to receive an ATS compatibility score.
- Highlights missing sections and keywords.
- Provides suggestions to improve your resume.
- Editor mode for direct resume text input and scoring.
- Supports synonym and section detection using NLP.
- Built with Flask, SpaCy, and Sentence Transformers.

## How It Works
1. Upload your resume and paste the job description.
2. The app extracts text from your resume and processes it using NLP.
3. It compares your resume to the job description for:
   - Section coverage
   - Keyword matching
   - ATS-friendliness
4. You receive a score and suggestions for improvement.

## Installation
1. Clone this repository.
2. Ensure Python 3.11+ is installed.
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   # or, if using poetry:
   poetry install
   ```
4. Download the spaCy English model:
   ```bash
   python -m spacy download en_core_web_sm
   ```

## Usage
Run the app locally:
```bash
python app.py
```
Visit [http://127.0.0.1:5000](http://127.0.0.1:5000) in your browser.

## Dependencies
- Flask
- sentence-transformers
- pymupdf
- scikit-learn
- nltk
- language-tool-python
- spacy

