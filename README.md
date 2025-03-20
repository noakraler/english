**Text Analysis for AAC Communication Boards**

## **Project Overview**

This project processes an academic English text (~500 words) and classifies words into five grammatical categories:
- **Nouns (NOUN)**
- **Verbs (VERB)**
- **Adjectives (ADJ)**
- **Adverbs (ADV)**
- **Connectives (CONNECTIVES)**

It then applies semantic clustering using SpaCy embeddings and KMeans. Finally, the results are visualized with bar charts, a pie chart, and a styled HTML table, which can be exported to PDF. The ultimate goal is to support the development of AAC (Augmentative and Alternative Communication) table.

## **Methodology**

1. **Data Acquisition**  
   - Downloads an academic English text arounf 500 words  
   - Cleans the text (removing punctuation and filtering unwanted words).

2. **Text Processing**  
   - **Tokenization**: Splits the text into individual words.  
   - **Lemmatization**: Uses NLTK and WordNet to reduce words to their base forms.  
   - **POS Tagging**: Assigns part-of-speech tags (NOUN, VERB, ADJ, ADV, CONNECTIVES).

3. **Classification**  
   - Sorts words into categories based on their POS tags.  
   - Selects the top 12 most frequent words from each category for deeper analysis.

4. **Semantic Clustering**  
   - Converts words into numerical vectors using SpaCy’s en_core_web_mb model.  
   - Groups words into 3 clusters (4 words each) per category using KMeans.  
   - Sorts words within each cluster by frequency.

5. **Visualization**  
   - **Bar Charts & Pie Chart**: Illustrates frequency distribution across categories.  
   - **HTML Table**: Displays clustered words, color-coded by category, with clear visual separation between clusters.  
   - **PDF Export**: Converts the HTML table to a PDF using pdfkit** and wkhtmltopdf.
   - 
## **Results**
- Identifies key frequent words in each grammatical category.  
- Clusters words based on semantic proximity to highlight similarities.  
- Creates a color-coded AAC table that can be directly used to build communication boards.

 Note on Custom Table Colors
GitHub’s native notebook preview does not fully render the custom HTML/CSS used in the AAC table. As a result, you may not see the colored cells when viewing this notebook on GitHub. To view the table with all its styling, please open the notebook in a Jupyter environment (locally or on Google Colab)

## **Technologies Used**
-  **Python** (for text processing)  
-  **NLTK & SpaCy** (for lemmatization, POS tagging, and word embeddings)  
-  **NumPy** (for numerical operations)  
   **Matplotlib & Seaborn** (for data visualization)  
   **pdfkit & wkhtmltopdf** (for converting HTML to PDF)

## **Future Work**
- **Develop an Auditory System**:Instead of written input, I would like to explore the possibility of doing something similar with auditory input.


