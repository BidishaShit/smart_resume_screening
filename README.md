#  Smart Resume Screening Pipeline

An AI-powered resume screening system that automates candidate evaluation, ranking, and reporting. This tool processes PDF resumes, predicts hiring suitability using a trained ML model, and generates a structured multi-sheet Excel report.

---

##  Features

-  Resume Parsing – Extracts data from PDF resumes  
-  Machine Learning Model – Predicts hiring decisions  
-  Candidate Ranking – Scores and ranks candidates automatically  
-  AI Insights – Generates hiring comments & probabilities  
-  Excel Report Export – Multi-tab structured report  
-  Styled Excel Output – Color-coded hiring decisions  

---

##  Tech Stack

- Python  
- Pandas  
- Scikit-learn  
- OpenPyXL  
- PDF Parsing Libraries  

---

##  Project Structure

```
├── training_data.csv / .xlsx
├── resumes/
├── screening_report.xlsx
├── main.py
```

---

##  How It Works

1. Load Training Data  
2. Train Classifier  
3. Extract Resume Data  
4. Predict Hiring Decisions  
5. Rank Candidates  
6. Export Excel Report  


---

##  Usage

### Run in Jupyter

```python
run_pipeline(
    training_file="path/to/training.csv",
    resume_folder="path/to/resumes",
    output_excel="output.xlsx",
    top_n=10
)
```

### Run via CLI

```bash
python main.py --training training.csv --resumes resumes/ --output report.xlsx --top_n 10
```

---

##  Output

- Summary Sheet  
- Role-wise Sheets  
- All Candidates Sheet  

Includes:
- Rank, Score, Name, Role  
- Skills, Experience, Education  
- Hire Probability & Decision  
- Contact Info  

---

##  Limitations

- Depends on training data quality  
- Resume parsing may vary  
- Possible model overfitting  

---

##  Future Improvements

- NLP-based parsing (BERT/LLMs)  
- Web interface  
- Explainable AI  

---

