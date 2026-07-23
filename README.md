# Bank Marketing Prediction

A clean and beginner-friendly machine learning project that predicts whether a bank client will subscribe to a term deposit (`y`) using the **Bank Marketing** dataset.

This project uses a **Decision Tree Classifier** from scikit-learn, along with simple preprocessing and model evaluation.

## Project Overview

The script:

- Loads `bank.csv` (semicolon-separated format)
- Encodes categorical features using `LabelEncoder`
- Splits the data into train/test sets
- Trains a `DecisionTreeClassifier`
- Evaluates predictions with accuracy and classification report
- Visualizes the trained decision tree

## Project Structure

```text
Bank-Marketing/
├── bank.csv
├── bank_marketing.py
└── README.md
```

## Requirements

- Python 3.8+
- pandas
- scikit-learn
- matplotlib

Install dependencies:

```bash
pip install pandas scikit-learn matplotlib
```

## How to Run

From the project folder, run:

```bash
python bank_marketing.py
```

## Expected Output

When you run the script, you will see:

- Encoded column data types
- Predicted labels for the test set
- Accuracy score
- Full classification report (precision, recall, f1-score)
- A plotted decision tree visualization

## Model Used

- **Algorithm:** Decision Tree Classifier
- **Train/Test Split:** 80/20
- **Random State:** 42

## Notes

- `LabelEncoder` is used directly on all object columns for simplicity.
- For production-grade modeling, consider:
  - one-hot encoding with `ColumnTransformer`
  - hyperparameter tuning (`max_depth`, `min_samples_split`, etc.)
  - cross-validation for more reliable performance

## Future Improvements

- Add feature importance chart
- Save the trained model with `joblib`
- Add confusion matrix and ROC-AUC (if applicable)
- Convert script into a notebook or modular package structure

## License

This project is for educational and learning purposes.
