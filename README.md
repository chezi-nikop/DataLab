# 🔍 LinkedIn Career Recommender

This project helps LinkedIn users discover *relevant companies, **job opportunities, and **online courses* based on their most recent position. The system is built from *three independent modules*, supported by a web scraping component for course data collection.

---

## 👨‍💻 Team Members
- Yitzhak Danan 
- Yechezkel Nikop
- Rafael Levi

---

## 📁 Project Structure

> 💡 *Each notebook is independent and can be executed on its own.*

### ⿡ project_yechezkel_part_1.ipynb – Company Matching  
Receives the user's most recent company and returns three similar companies using a classification model based on TF-IDF of company descriptions, size, and number of followers.  
All data processing was done using *Apache Spark, similar to **Homework 3* in the course.  
- ❌ No demo included (can be added manually if needed)

### ⿢ project_itzik_part_2.ipynb – Job Recommendation  
Ranks job openings from matched companies using BERT-based semantic similarity, location proximity, salary normalization, and job type weighting.  
- ✅ Includes a complete demo run at the end

### ⿣ project_refael_part_3.ipynb – Course Recommendation  
Recommends relevant online courses for each job based on job descriptions.  
- ✅ Includes a demo run at the end

### 🕸 project_scraping.ipynb – Scraping Module  
Contains the scraping logic used to collect online course data (e.g., from Coursera and Udemy).  
The scraping was done using *Bright Data proxies* to bypass site limitations and ensure access to real-time course listings.

> ⚠ *Note:* The scraped course data is *not included* in the repository due to data usage restrictions.

---

## 📂 Data Access

The repository does *not* contain any raw data from LinkedIn or Bright Data, in accordance with course regulations and data usage policies.

However, the following *processed and publicly available datasets* are shared for demonstration purposes:

1. courses.pkl – A filtered and cleaned dataset of online courses collected via web scraping using Bright Data proxies.  
   ✅ Includes only high-level metadata (title, description, rating, etc.), no raw HTML or platform-specific identifiers.

2. linkedin_124k_kaggle_filterd.csv – A public job listing dataset downloaded from Kaggle and filtered to include relevant job postings for testing the recommendation system.

These files are hosted in a private folder accessible here:  
🔗 [https://drive.google.com/drive/folders/1OnR9EMFlNNsNN3u2Hl7QEkor_m_Q8sGV?usp=drive_link]

> ✅ Access permission should be set to: *"Anyone with the link can view"*  
> ❌ Do not include any raw LinkedIn or Bright Data files in the repository or in this folder.

---
## 📢 Project Video Demonstration

we created a short video presenting the project and explaining its components.

🔗 [🎬 Watch the demo video][https://drive.google.com/drive/folders/1ZnQMmPHOd507nDV-H_7NN7YzFmiRJQHa?usp=drive_link]

## ⚙ How to Run

Each notebook can be run separately in Jupyter or Google Colab.  
Please make sure the required dependencies are installed.

### Installation:
```bash
pip install pandas numpy scikit-learn transformers geopy torch matplotlib



