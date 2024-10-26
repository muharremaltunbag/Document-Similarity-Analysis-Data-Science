# Document-Similarity-Analysis-Data-Science

This project explores the computational efficiency of various document similarity algorithms, a critical area in data science applications like information retrieval, clustering, and natural language processing. Using a dataset derived from *War and Peace* by Leo Tolstoy, we analyze and benchmark different similarity measures, including Cosine and Jaccard, and experiment with optimization techniques such as parallel processing and Strassen's algorithm.

## Project Overview
The goal of this project is to understand the performance trade-offs between different similarity measures and optimization methods for large-scale document similarity computations. By analyzing both theoretical and empirical runtime complexities, this project provides insights into efficient ways to compute document similarity in data-intensive environments.

## Project Structure
- **`notebook.ipynb`**: Jupyter Notebook containing all code, analysis, and visualizations for each question in the project. 
- **`data/`**: Directory containing `data2023.csv`, the main dataset used in this project.
- **`docs/`**: Directory with additional reference documents:
  - `Getting started 2023.pdf`: Instructions on loading and preparing the dataset.
  - `Muharrem Altunbag_284362_Report T1.pdf`: Detailed project report covering all findings and methods in the Jupyter notebook.
- **`requirements.txt`**: List of required packages to install for running the notebook.

> **Note**: All analysis, code, and explanations are thoroughly documented in the `Muharrem Altunbag_284362_Report T1.ipynb` file, with supporting information available in the `docs/` directory.

## Key Questions Explored
1. **Cosine Similarity Analysis**: 
   - **Objective**: Evaluate the theoretical and empirical performance of Cosine similarity for comparing document pairs.
   - **Tasks**: Calculate cosine similarity using both `numpy` and a custom implementation, time their performance, and visualize results.
   
2. **Jaccard Similarity Analysis**:
   - **Objective**: Examine the Jaccard similarity's theoretical complexity and runtime performance when comparing document pairs.
   - **Tasks**: Convert frequency data to binary format for Jaccard computation, measure runtimes, and discuss scalability.

3. **All-Pairs Similarity Computation**:
   - **Objective**: Analyze the complexity and performance of all-pairs similarity calculations for large datasets.
   - **Tasks**: Evaluate both Cosine and Jaccard similarity measures for all document pairs, compare runtime growth, and identify efficient methods for scaling.

4. **Parallel Processing**:
   - **Objective**: Implement parallel processing to speed up all-pairs similarity calculations.
   - **Tasks**: Use `joblib` to distribute similarity computations across multiple CPU cores and empirically measure the speedup.

5. **Strassen’s Algorithm for Matrix Multiplication**:
   - **Objective**: Investigate Strassen's algorithm's efficiency for calculating all-pairs cosine similarities on large datasets.
   - **Tasks**: Compare Strassen's algorithm to standard matrix multiplication, assess speed improvements, and discuss when it’s beneficial for large data matrices.

## Installation and Setup
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/Document-Similarity-Analysis-Data-Science.git
   cd Document-Similarity-Analysis-Data-Science
