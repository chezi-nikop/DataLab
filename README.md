# 🔍 LinkedIn Career Recommender

This project helps LinkedIn users discover *relevant companies, **job opportunities, and **online courses* based on their most recent position. The system is built from three *independent* Jupyter notebooks, each focusing on a different stage of the recommendation pipeline.

---

## 👨‍💻 Team Members
Yechezkel Nikop
Itzhak Danan
refael Levi

---

## 📁 Project Structure

> 💡 *Each part is independent and can be executed separately.*

### ⿡ project_yechezkel_part_1.ipynb – Company Matching
Finds companies that are relevant to a user's latest job, based on industry, company type, and size.  
Built using PySpark to process LinkedIn company and user data.

- ❌ *This notebook does not include a runnable example.*
- 🛠 You may add a test profile manually to simulate the process.

---

### ⿢ project_itzik_part_2.ipynb – Job Recommendation
Ranks job postings from the matched companies using multiple criteria:
- Semantic similarity (BERT-based cosine similarity between profile and job)
- Geographic proximity (via geopy)
- Salary normalization
- Job type weighting

- ✅ *Includes a complete demo run at the end of the notebook.*

---

### ⿣ project_refael_part_3.ipynb – Course Recommendation
Recommends online courses based on job descriptions using a dataset of thousands of training programs.

- ✅ *Includes a demo run at the end of the notebook.*

---

## ⚙ How to Run

Each notebook runs independently and can be executed in Jupyter or Google Colab.

### Installation
Install the required Python packages:

```bash
pip install pandas numpy scikit-learn transformers geopy torch matplotlib

---

## 📂 Data Access

The processed data files used in this project are available at the following secure location:

🔗 [Private Google Drive Link](https://drive.google.com/your_link_here)

> ⚠ Original LinkedIn / BrightData raw datasets are *not* included in the repository, in accordance with the project policy.

---

### 🕸 project_scraping.ipynb – Scraping Module  
This notebook contains the code used to collect online course data using automated web scraping. The scraping was performed via *Bright Data proxies*, enabling access to course platforms such as Coursera and Udemy as part of the data collection process.
