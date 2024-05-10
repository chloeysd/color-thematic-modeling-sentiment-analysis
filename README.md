# color-thematic-modeling-sentiment-analysis

## Project Overview
This project is designed to analyze and present information related to color extracted from Wikipedia. It combines multi-step data processing and visualization techniques to leverage open data for creating an interactive interface that showcases topic modeling, network visualization, sentiment analysis, and data-driven word clouds.

## Environment Setup
Ensure the following tools and libraries are installed to run this project:
- **Python**
- **Libraries**: requests, BeautifulSoup, nltk, pandas, sklearn, TextBlob, NetworkX, matplotlib, word cloud, Tkinter

## Project Structure
- `code&data/`: Contains datasets and datasheets generated from Wikipedia and Python scripts for each step of the workflow.
- `image/`: Stores visualization outputs such as network graphs and word clouds.

## Running the Project
1. **Web Scraping Wikipedia (`1_webscrape_wikipedia.ipynb`)**:
   - Extracts datasets from Wikipedia using modified classroom code with a custom user agent and enhanced text extraction. Outputs are stored in `data/my-data`.

2. **Topic Modeling (`2_LDA_Topic_Analysis.ipynb` & `2_LSA_Topic_Analysis.ipynb`)**:
   - Performs LDA and LSA topic modeling. LDA results are used for further analysis.

3. **Network Visualization (`3_network_visualization.ipynb`)**:
   - Visualizes LDA results as network graphs with custom colors and node sizing by weight. Outputs are stored in `image/`.

4. **Sentiment Keyword Analysis (`4_sentiment_keyword.ipynb`)**:
   - Conducts sentiment analysis based on LDA keywords using TextBlob, combining document sentiment scores with TF-IDF values for keyword sentiment scoring.

5. **Word Cloud Generation (`5_wordcloud.ipynb`)**:
   - Integrates results from Steps 3 and 4 to create word clouds for each topic, with word size representing weight and color saturation representing sentiment. Outputs are stored in `image/`.

6. **Interactive GUI Interface (`6_tool copy.ipynb`)**:
   - Combines all information to create analytical texts and a GUI interface using Tkinter with three interactive windows.

## Acknowledgments
This code was adapted from classroom content, online resources, and consultations with a large language model for error resolution. Proper citations are provided within the code comments.

