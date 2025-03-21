**Text Analysis for AAC Communication Boards**

## **Project Overview**

This project processes an academic English text (~500 words) and classifies words into five grammatical categories nonans, verbs, adjectives, adverbs and connectives.

 after, it applies semantic clustering. Finally, the results are visualized in a styled HTML table, which can be exported to PDF. The ultimate goal is to support the development of AAC (Augmentative and Alternative Communication) table.

## **Methodology**

1. **Data Acquisition**  
   - upload an  English text arounf 500 words  
   - Cleans the text
     
2. **Text Processing**   : Tokenization, Lemmatization anf POS Tagging


3. **Classification**  
   - Sorts words into categories based on their POS tags.  
   - Selects the top 12 most frequent words from each category and analyzed them
      
4. **Semantic Clustering**  
   - Converts words into numerical vectors.  
   - Groups words into 3 clusters (4 words each) per category using KMeans.  
   - Sorts words within each cluster by frequency.

5. **Visualization**  
   - **Bar Charts & Pie Chart**: Illustrates frequency  and frequency distribution within  the categories .  
   - **HTML Table**: Displays clustered words, color-coded by category, with clear visual separation between clusters.  
   - **PDF Export**: Converts the HTML table to a PDF and download it.
      
## **Results**

the result show the identifies key frequent words in each grammatical category. and the clustring  words groups based on  their semantic proximity.  that creates a color-coded AAC table that can be directly used to build communication boards.


   **important note**
Custom Table Colors=  GitHub’s native notebook preview does not fully render the custom HTML/CSS used in  this AAC table. As a result, you may not see  in this GItHub the colored cells when viewing this notebook.  in order to view the table with all its styling, you can  open the notebook in a Jupyter environment (locally or on Google Colab)

## **Technologies Used**
-  **Python** (for text processing)  
-  **NLTK & SpaCy** (for lemmatization, POS tagging, and word embeddings)  
-  **NumPy** (for numerical operations)  
   **Matplotlib & Seaborn** (for data visualization)  
   **pdfkit & wkhtmltopdf** (for converting HTML to PDF)

## **Future Work**
- **Develop an Auditory or children costume made System**:Instead of written input, I would like to explore the possibility of doing something similar with auditory input. or input that is more suitable for children 


