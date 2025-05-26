# Resume Matcher Application

**Author:**  Amitesh Sinha

## Executive Summary

The Resume Matcher Application leverages Natural Language Processing (NLP) techniques to analyze and quantify how well a candidate's resume aligns with a specific job description. By extracting and comparing technical and soft skills, the tool provides match scores and visual insights, facilitating automated resume screening and profile matching.

## Rationale

In the competitive job market, recruiters often face the daunting task of sifting through numerous resumes to find the right candidate. This application addresses the need for an efficient, automated solution to assess resume relevance, thereby streamlining the recruitment process and reducing manual effort.

## Research Question

How can NLP techniques be utilized to effectively compare and score the alignment between a candidate's resume and a job description?

## Data Sources

- Resumes and job descriptions stored in the `Data/` folder.
- Supported file formats: `.pdf`, `.docx`, and `.txt`.

## Methodology

**Data Extraction:**  
- Utilize `pdfplumber` for PDFs, `python-docx` for Word documents, and plain text reading for `.txt` files to extract textual content.

**Pre-processing:**  
- Tokenize text, remove stopwords, and clean data to prepare for analysis.

**Exploratory Data Analysis (EDA):**  
- Generate statistics such as document counts and word counts.  
- Visualize data using histograms and word clouds to identify common terms.

**Skills & Keywords Extraction:**  
- Extract technical and soft skills from both resumes and job descriptions.  
- Compute overlap and relevance between extracted skills.

**Resume Fitness Scoring:**  
- Calculate match scores for hard skills, soft skills, and overall alignment.  
- Highlight top-matched skills for each resume.

**Visualization:**  
- Create word clouds, bar charts for matched skills, and optional cosine similarity heatmaps to present findings.

## Results

The application successfully processes various resume formats, extracts pertinent skills, and quantifies the alignment with job descriptions. Visual tools like word clouds and bar charts provide intuitive insights into the matching process, aiding recruiters in decision-making.

## Next Steps

- Implement automatic extraction of bigrams and trigrams (e.g., "machine learning", "project management").
- Enable comparison of resumes across multiple job descriptions.
- Incorporate extraction of education, experience, and contact information.
- Develop features to detect missing sections or inconsistencies in resumes.
- Integrate pretrained models for named entity recognition (NER) to enhance information extraction.

## Outline of Project

- [Link to notebook](https://github.com/amiteshks/resume_matcher/blob/main/resume_match.ipynb)

### Contact and Further Information

For more details, please refer to the project's GitHub repository: [Resume Matcher Application](https://github.com/amiteshks/resume_matcher)



