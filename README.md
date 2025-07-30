# Logistic Regression: Insurance Purchase Prediction

## Overview
This project implements a logistic regression model to predict whether a customer purchases insurance, using features such as age and other relevant attributes. The complete machine learning workflow is provided in a Jupyter Notebook.

## Project Structure
- `notebook.ipynb`: Step-by-step implementation and explanations.
- `flowchart.png`: High-definition flowchart illustrating the workflow.
- `insurance_data.csv`: Sample data for model training and testing.
- `README.md`: Project description, usage instructions, and methodology.

## Workflow: Step-by-Step

1. **Start**
2. **Import & Load Data**
    - Import required libraries (`pandas`, `numpy`, `matplotlib`, `seaborn`).
    - Load the dataset into a DataFrame.
3. **Data Exploration & Preprocessing**
    - Display data samples and check for missing values.
    - Clean and preprocess data as necessary.
4. **Feature Selection & Splitting**
    - Choose relevant features and define the target variable.
    - Separate features (`X`) and labels (`y`).
5. **Model Training**
    - Initialize and fit a Logistic Regression model using scikit-learn.
6. **Prediction (Probability Output)**
    - Model computes the probability of the target outcome for each sample:
      - Linear combination: *z = w₁x₁ + ... + wₙxₙ + b*
      - Apply sigmoid (logistic) function: *p = 1 / (1 + e^(–z))*
      - *p* is the estimated probability of the target being 1.
7. **Thresholding (Logical Decision)**
    - Compare predicted probability to a threshold (commonly 0.5).
    - If *p ≥ 0.5* → Classify as 1 (“Yes”, bought insurance)
    - If *p < 0.5* → Classify as 0 (“No”, did not buy insurance)
8. **Model Evaluation**
    - Evaluate using accuracy, precision, recall, F1-score, etc.
9. **End**

## Flowchart
See the included `flowchart.png` for a visual overview of the pipeline and the key logical decision point.

## Requirements
- Python 3.7+
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage
1. Clone the repository.
2. Open `notebook.ipynb` and run through each cell.
3. Review `flowchart.png` for a conceptual overview.

## License
This project is licensed under the MIT License.

## Contact
For questions, feel free to open an issue or submit a pull request.

---

**Professional Tips:**
- The flowchart distinguishes between continuous output (probability) and binary decision (yes/no).
- The workflow follows best practices and is easy to adapt for other binary classification tasks.

Feel free to customize this template for your project!
