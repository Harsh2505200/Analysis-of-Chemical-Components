# Analysis of Chemical Components

This project analyzes cosmetic products, particularly moisturizers for dry skin, by tokenizing their ingredients and applying dimensionality reduction through t-SNE. It also provides an interactive visualization of the data using Bokeh's scatter plots.



## Dataset

The dataset contains information on various cosmetic products, including details like ingredients, price, rank, and brand.

### Features:
- **Label**: The product category (e.g., Moisturizer, Shampoo).
- **Brand**: The brand of the product.
- **Name**: The name of the product.
- **Price**: The price of the product.
- **Rank**: User ratings or ranking of the product.
- **Ingredients**: A list of ingredients used in the product.
- **Combination**: Indicates if the product is suited for combination skin (1 for Yes, 0 for No).
- **Dry**: Indicates if the product is suitable for dry skin (1 for Yes, 0 for No).
- **Normal**: Indicates if the product is suitable for normal skin (1 for Yes, 0 for No).
- **Oily**: Indicates if the product is suitable for oily skin (1 for Yes, 0 for No).
- **Sensitive**: Indicates if the product is suitable for sensitive skin (1 for Yes, 0 for No).




## Workflow

1. **Data Preprocessing**:
   - Loaded the dataset using pandas.
   - Filtered the dataset to include only moisturizers for dry skin.
   
2. **Ingredient Tokenization**:
   - Tokenized the ingredients for each product and created a dictionary mapping each unique ingredient to an index.

3. **Document-Term Matrix (DTM)**:
   - Built a Document-Term Matrix using one-hot encoding to represent each product's ingredients.

4. **Dimensionality Reduction (t-SNE)**:
   - Applied t-SNE to reduce the dimensionality of the dataset and enable visualization in 2D.

5. **Data Visualization**:
   - Used Bokeh to create an interactive scatter plot based on the t-SNE results.
   - Added hover tools to the plot to display product details such as name, brand, price, and rank.

6. **Product Comparison**:
   - Compared ingredients between two similar products to highlight their differences.



## Key Libraries

This project utilizes the following libraries:

- **pandas**: For data manipulation and analysis.
- **numpy**: For numerical computations.
- **scikit-learn**: For implementing t-SNE (Dimensionality Reduction).
- **bokeh**: For creating interactive visualizations.
- **matplotlib**: For static plotting (optional).



## Project Insights

This project provides valuable insights into the similarities and differences between cosmetic products based on their ingredients. The interactive visualizations allow for easy exploration of the dataset, aiding in the discovery of patterns and trends in the product ingredients.
