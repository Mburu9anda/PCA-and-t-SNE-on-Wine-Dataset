#  Wine Dataset: PCA & t-SNE Analysis

This project explores dimensionality reduction techniques using the Wine dataset.

## Objectives

- Apply PCA and analyze explained variance
- Compare Logistic Regression performance (Original vs PCA)
- Visualize PCA components
- Explore t-SNE with different perplexities
- Compare clustering quality

##  Dataset

- Source: sklearn.datasets.load_wine
- Classes: 3 wine types
- Features: 13 chemical properties

##  Techniques Used

### 1. PCA (Principal Component Analysis)
- Reduced dimensionality while preserving variance
- Selected components covering 95% variance

### 2. Logistic Regression
- Compared performance on:
  - Original data
  - PCA-reduced data

### 3. t-SNE
- Tested perplexities:
  - 5 (local structure)
  - 30 (balanced)
  - 100 (global structure)


##  Results

| Model | Accuracy |
|------|--------|
| Original Data | ~0.97 |
| PCA Reduced | ~0.97 |

PCA retained performance while reducing dimensions.


## Visualization Insights

### PCA
- Clear separation between wine classes
- Linear structure

### t-SNE
- Perplexity 5 → more scattered clusters
- Perplexity 30 → best cluster separation
- Perplexity 100 → overly compressed clusters


## Conclusion

- PCA is effective for dimensionality reduction with minimal loss
- t-SNE provides better visual clustering
- Perplexity tuning is critical in t-SNE

