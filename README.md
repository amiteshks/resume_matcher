# Resume Matcher Application

This project analyzes how well a candidate's resume matches a given job description using Natural Language Processing (NLP) techniques. It extracts, compares, and scores technical and soft skills from resumes and job descriptions, providing insights for automated resume screening and profile matching.


## Features

- Load resumes in `.pdf`, `.docx`, and `.txt` formats
- Extract text using `pdfplumber`, `python-docx`, or plain text reading
- Clean and tokenize resume and job description content
- Extract technical and soft skills
- Compare skills using:
  - Exact keyword matching
  - TF-IDF
  - N-gram analysis
- Calculate skill match scores and resume fitness
- Generate visualizations:
  - Word clouds
  - Skill match bar charts
  - Cosine similarity scores

## How It Works

### Section 1: Data
- Resumes and job descriptions are stored in the `Data/` folder.
- Accepts `.pdf`, `.docx`, and `.txt` file formats.

### Section 2: Pre-processing
- Extracts raw text content from resumes and job descriptions.
- Tokenizes, removes stopwords, and cleans the data.

### Section 3: Exploratory Data Analysis (EDA)
- Displays basic stats: document counts, word counts, histogram of lengths.
- Shows most common words using frequency and word cloud visualizations.

### Section 4: Skills & Keywords Extraction
- Extracts technical and soft skills from text.
- Computes overlap between job requirements and resume skills.

### Section 5: Resume Fitness Scoring
- Calculates:
  - Hard skill match score
  - Soft skill match score
  - Overall resume matching score
- Displays top matched skills per resume.

### Section 6: Visualization
- Word clouds
- Bar charts of matched skills
- Cosine similarity heatmap (optional)

## Future Enhancements

- Automatically extract bigrams and trigrams (e.g., "machine learning", "project management")
- Compare resumes across multiple job descriptions
- Include education, experience, and contact info extraction
- Detect missing sections or inconsistencies
- Use pretrained models for named entity recognition (NER)

## Technologies Used

- Python
- pandas, numpy
- nltk, spaCy
- sklearn (TF-IDF, cosine similarity)
- matplotlib, seaborn, wordcloud, plotly

## How to Run

1. Clone the repo:


