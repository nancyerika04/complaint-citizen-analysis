# complaint-citizen-analysis
# Citizen Complaints Analysis with NLP

##  Overview
This project analyzes citizen complaints (NYC 311 Service Requests dataset) using Natural Language Processing (NLP).  
The goal is to identify the main themes in the complaints and group similar complaints to help decision-makers better understand citizens’ concerns.

##  Dataset
- Source: NYC 311 Service Requests (Open Data)
- Key columns used:
  - **Complaint Type**: general category of the complaint
  - **Descriptor**: detailed description of the complaint

##  Methods
1. **Data Cleaning & Preprocessing**
   - Lowercasing, removing special characters
   - Stopwords removal
   - Lemmatization with spaCy
2. **Vectorization**
   - CountVectorizer (for topic modeling)
   - TF-IDF (for clustering)
3. **Models**
   - Latent Dirichlet Allocation (LDA) → extract main topics
   - K-means clustering → group similar complaints
4. **Visualization**
   - Wordcloud of frequent words
   - Top complaint types
   - PCA visualization of clusters

##  Results
- LDA topics show main citizen issues such as **noise**, **illegal parking**, and **derelict vehicles**.
- K-means clusters confirm complaint groupings by type.
- Wordcloud highlights the most frequent terms (e.g., *noise*, *parking*, *blocked*).

##  How to Run
1. Open the notebook in Google Colab.
2. Upload or mount the dataset.
3. Run cells step by step (from Import → Cleaning → Vectorization → Models → Visualization).

##  Conclusion
This project demonstrates how NLP can extract valuable insights from unstructured text data,  
helping municipalities prioritize actions and respond more effectively to citizens' concerns.

