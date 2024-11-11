# Flybondi Reviews

Taking a deep dive and understanding the strengths and weaknesses of the business based on online reviews.


### Data Cleaning Pipeline for Flybondi Reviews

This cleaning pipeline processes the Flybondi reviews to prepare the data for analysis. The image below show a preview of the data recollection process.

![cleaingn_pipeline_img](./res/image.png)


#### Steps

1. **Initial Cleaning with Pandas**  
   - Drop unnecessary columns.
   - Remove duplicate entries.
   - Normalize columns like `Rating` and `Likes`.
   - Convert text to lowercase for consistency.

2. **Review Content Check**  
   - Verify if each review has a title. If so, concatenate the title with the review content.

3. **Relevance Scoring**  
   - For reviews without a title, generate a `Relevance Score` to prioritize them in the analysis.

4. **Language Detection and Translation**  
   - Detect the language of each review.
   - Translate non-Spanish reviews to Spanish using Google Translate API for uniform language analysis.

5. **Text Processing with NLP Libraries**  
   - Use Stanza and NLTK to clean the review text further:
     - Remove stopwords.
     - Lemmatize words to their root form for better NLP processing.

This pipeline ensures the reviews are cleaned, normalized, and ready for further sentiment analysis or business insights extraction.

### Processing and Analysis

link al drive: https://drive.google.com/drive/u/1/folders/1urDqKTYl_T_UYg0KQg_PRr_GvVs60TYA