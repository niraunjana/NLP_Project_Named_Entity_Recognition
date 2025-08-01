# NLP_Project_Named_Entity_Recognition
## Resume Information Extraction using Named Entity Recognition (NER)

## Objective

The objective of this project is to design and implement an NLP-based system that can automatically extract structured information from unstructured resume documents (in .txt or .pdf formats).
This system simulates a real-world HR automation task using Named Entity Recognition (NER) to identify:

1. 👤 Name

2. 💼 Skills

3. 🎓 Degree(s)

4. 🏫 Institutions

5. 🕒 Work Experience

## What is Named Entity Recognition (NER)?

Named Entity Recognition (NER) is a Natural Language Processing (NLP) technique used to locate and classify named entities in text into predefined categories such as person names, organizations, locations, expressions of times, quantities, and more.

In this project, NER is leveraged to identify entities specific to resumes and job profiles, using both:

Pre-trained NER models (like SpaCy)

Rule-based matching (for domain-specific keywords like skills, degrees, etc.)

## Tools & Technologies Used

Python - Main programming language

SpaCy - Used for NLP and custom NER modeling

PyMuPDF (fitz) - Used for PDF text extraction

Regex (re) - Pattern matching for rule-based extraction

pandas - Data structuring and tabular export (CSV, JSON)

nltk - Tokenization and text preprocessing


## Text Extraction

1. PDF resumes are parsed using PyMuPDF to extract raw text.

2. Text files are read directly.

3. Text Preprocessing

---> Cleaning, tokenization, and removal of stopwords.

---> Normalization of text (lowercasing, punctuation removal).

---> Named Entity Recognition

4. Uses SpaCy’s en_core_web_sm model to identify:

---> PERSON → Candidate names

---> ORG → Institutions and employers

---> DATE → Work durations

5. Uses custom rules and regex to extract:

---> Degrees (e.g., B.Tech, MBA)

---> Skills (via predefined keyword set)

---> Work Experience descriptions

---> Structured Output Generation

6. Extracted data is converted to JSON or CSV format for further processing or storage.

## Output 

<img width="755" height="126" alt="image" src="https://github.com/user-attachments/assets/f9b6b984-ce2e-45bf-b2d6-b6b4ec7f7146" />


<img width="676" height="91" alt="image" src="https://github.com/user-attachments/assets/8175685e-9e1e-49c3-84f5-5b3b06382f2e" />


<img width="1000" height="561" alt="image" src="https://github.com/user-attachments/assets/39108b40-cf70-49bf-8bda-2fdd3c33cb14" />

## Accuracy 

<img width="560" height="227" alt="image" src="https://github.com/user-attachments/assets/4ef9cd0b-225a-4b27-a434-a4c6cd9518c8" />

## Saved Model

<img width="513" height="126" alt="image" src="https://github.com/user-attachments/assets/dfc528d5-421b-4ede-a2d6-53a3e102498e" />


## Requirements (requirements.txt)

1. nginx
   
2. Copy
   
3. Edit
   
4. spacy
   
5. pymupdf
   
6. nltk
   
7. pandas
   

## Project Highlights

Fully automatic parsing of resumes (PDF/Text)

Combination of SpaCy's ML models and rule-based matching

Structured and clean output in JSON/CSV formats

Can be extended for HR systems and ATS (Applicant Tracking Systems)


## Result

The system successfully extracted relevant structured information from multiple resumes with high accuracy, demonstrating the power of combining NER models with custom rule-based logic for real-world resume screening automation.

