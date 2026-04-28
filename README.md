# CiteWise: Research Paper Citation Analyzer

## Project Idea

CiteWise is an automated system designed to improve the quality of research documents by analyzing and validating citations.
It extracts key information from a research paper such as metadata, references, and citations, and checks whether the citations used in the paper are valid.

The aim is to reduce manual effort in citation verification and ensure accurate referencing in academic work.

---

## Tools & Technologies Used

* **Python** – Core programming language
* **Google Colab** – Development and execution
* **PyMuPDF (fitz)** – PDF text extraction
* **Regex (re)** – Pattern matching
* **Scikit-learn (TF-IDF)** – Keyword extraction
* **GitHub** – Version control
* **Mendeley** – Reference management & citation organization

---

## Role of Mendeley (Important)

Mendeley is used as a **reference management tool** in this project.

### 🔹 What it does:

* Stores and organizes research papers (PDFs)
* Maintains structured reference data (author, year, title)
* Helps in generating citations and bibliographies

### 🔹 In this project:

* Mendeley acts as a **reference database**
* References (author + year) can be exported or used to create `references.json`
* This improves:

  * ✔ Citation accuracy
  * ✔ Validation reliability
  * ✔ Structured referencing

---

## How It Works

### 1️⃣ Input

* User uploads a research paper (PDF)
* Optionally provides `references.json` (from Mendeley or manually created)

---

### 2️⃣ Metadata Extraction

The system extracts:

* Title
* Authors
* Year
* Keywords
* Abstract

---

### 3️⃣ Citation Detection

* Detects numeric citations like `[1], [2], [3]`
* Can also support author-year citations

---

### 4️⃣ Reference Extraction

* Extracts references from PDF
* OR uses structured data from Mendeley (`references.json`)

---

### 5️⃣ Citation Verification

* Matches citations with references
* Classifies into:

  * ✅ Valid
  * ❌ Invalid

---

### 6️⃣ Output Generation

The system generates:

* Metadata summary
* Citation count
* Valid/Invalid classification
* Citation-reference mapping
* Final structured output

---

## Project Structure

```
CiteWise/
│
├── CiteWise.ipynb        # Main Colab notebook (core logic)
├── output.txt            # Generated output (results)
├── sample_paper.pdf      # Sample research paper
├── README.md             # Project documentation
```

---

## Key Features

* Automatic metadata extraction
* Citation detection and validation
* Works on real research PDFs
* Supports external reference database (Mendeley)
* Generates structured output

---

## Future Improvements

* Convert `[1] → (Author, Year)` automatically
* Highlight missing citations in text
* Export results as PDF/Word
* Build a web-based interface
* Direct integration with Mendeley API

---

## Conclusion

CiteWise simplifies citation analysis by combining PDF processing, reference management, and validation techniques.
With integration of tools like GitHub and Mendeley, it ensures better accuracy, organization, and reproducibility in research workflows.

---
