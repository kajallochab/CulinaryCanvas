# CulinaryCanvas

### Overview

Culinary Canvas is an information retrieval system course project aimed at providing a recipe search algorithm. The system allows users to input a list of ingredients or categories and retrieves relevant recipes based on similarity scores calculated using TF-IDF matrices. The project utilizes topic modeling techniques such as Latent Dirichlet Allocation (LDA) and Non-negative Matrix Factorization (NNMF) for extracting topics from a dataset of recipes. Additionally, keyword extraction using TextRank is employed to summarize topics effectively.


### How it Works

1. Data Preprocessing: The project begins by loading a dataset containing food ingredients and recipes. Missing values are handled, and rows containing only punctuation or numbers are dropped. Recipes with insufficient instructions are also removed.

2. Topic Modeling: LDA and NNMF algorithms are applied to extract topics from the dataset. Topic distributions for documents and words are generated, and keyword extraction is performed using TextRank.

3. Querying Algorithm: The system provides a search algorithm that calculates similarity scores between user queries and recipes' titles, instructions, and keywords. TF-IDF matrices are utilized, and the search algorithm is tested with various queries to demonstrate functionality.

4. Conclusions and Future Work: The README concludes with a summary of project outcomes, highlighting the effectiveness of leveraging original recipe text and proposing future improvements such as incorporating GloVe embeddings, LDA2Vec topic extraction, and web scraping for dynamic recipe updates.


### Workflow

Data Preprocessing: Load the dataset, handle missing values, and remove irrelevant rows.

Topic Modeling: Apply LDA and NNMF algorithms to extract topics from the dataset. Perform keyword extraction using TextRank.

Querying Algorithm: Develop a search algorithm that calculates similarity scores between user queries and recipes' titles, instructions, and keywords.

Testing: Test the search algorithm with various queries and ranked query ingredients to ensure functionality.


### Future Work

Several enhancements and future directions have been identified for the Culinary Canvas project:

Incorporating GloVe embeddings and LDA2Vec topic extraction for improved topic modeling.

Implementing web scraping to dynamically update the recipe dataset and keep it current.

Developing a user interface to facilitate user interaction and enhance user experience.

Exploring dense word embeddings and semantic similarity measures to capture nuanced relationships between ingredients and recipes.

Expanding the scope of keywords associated with each topic to ensure comprehensive search functionality.


### Getting Started

To get started with Culinary Canvas, follow these steps:

1. Clone the repository to your local machine.
2. Install the necessary dependencies listed in the requirements.txt file.
3. Run the provided Python scripts to preprocess data, train topic models, and implement the search algorithm.
4. Test the algorithm with various query inputs to evaluate its performance.


### Contributors
    [Your Name]
    [Collaborator 1]
    [Collaborator 2]

### License
This project is licensed under the MIT License - see the LICENSE.md file for details

### Dataset
Dataset used can be found on kaggle under the title: Food Ingredients and Recipes Dataset with Images
Link: https://www.kaggle.com/datasets/pes12017000148/food-ingredients-and-recipe-dataset-with-images

The dataset contains a CSV file and a zipped folder, consisting of 13,582 images and rows respectively.

The CSV file, Food Ingredients and Recipe Dataset with Image Name Mapping, contains 5 columns, as follows:

- Title: Represents the Title of the Food Dish.
- Ingredients: Contains the ingredients as they were scraped from the website.
- Instructions: Has the recipe instructions to be followed to recreate the dish.
- Image_Name: Has the name of the image as stored in the Food Images zipped folder.
- Cleaned_Ingredients: Contains the ingredients after being processed and cleaned.
    
