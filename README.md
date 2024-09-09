# Loan Application Risk Prediction

This project focuses on predicting whether a two-wheeler loan application will be accepted or rejected based on various applicant details. The prediction is made using a classification model built in Python, leveraging machine learning techniques.

## Project Structure

- `Assignment_Train.csv`: Training data with labeled loan application status.
- `Assignment_Test.csv`: Test data without labeled loan application status, used for prediction.
- `Assignment_FeatureDictionary.xlsx`: A feature dictionary describing each variable in the training and test data.
- `BUREAU ASSIGNMENT.ipynb`: Jupyter Notebook containing the full workflow, including data exploration, feature engineering, model training, evaluation, and prediction.

## Approach

1. **Data Understanding**: The dataset includes both categorical and numerical features. A thorough data exploration step was conducted to understand feature distributions, relationships, and missing values.
   
2. **Data Preprocessing**:
   - Missing values were handled.
   - Categorical features were encoded for model compatibility.
   - Numerical features were scaled as needed.

3. **Modeling**:
   - A Random Forest classifier was selected for this task due to its robustness with mixed data types and ability to handle complex interactions between features.
   - Hyperparameter tuning was performed to optimize model performance.

4. **Evaluation**:
   - The model was evaluated using accuracy, precision, recall, F1-score, and ROC-AUC metrics.
   - Confusion matrix and ROC curves were plotted for performance visualization.

5. **Test Prediction**:
   - The final model was used to generate predictions for the test dataset, which were saved in the required format (`predictions.csv`).

## Visualizations

Several visualizations were created to better understand the data:
- **Categorical Feature Distribution**: Stacked bar plots were used to show how different categories, such as 'Marital Status' and 'Employer Type', are distributed across approved and declined applications.
- **Numerical Feature Distribution**: Histograms and pair plots helped reveal patterns for features like 'Cibil Score', 'Age', and 'Applied Amount', highlighting their impact on application status.
- **Correlation Heatmap**: A heatmap was plotted to display the relationships between various features and how they correlate with each other.

## Requirements

- Python 3.x
- Jupyter Notebook
- Libraries used:
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `seaborn`
  - `scikit-learn`

You can install the required packages using:

```bash
pip install -r requirements.txt
```

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/loan-risk-prediction.git
   cd loan-risk-prediction
   ```

2. Open the Jupyter notebook:
   ```bash
   jupyter notebook BUREAU ASSIGNMENT.ipynb
   ```

3. Follow the steps in the notebook to explore the data, train the model, and generate predictions.

4. The output file `predictions.csv` will contain the predictions for the test set.

## Results

- The final Random Forest model achieved an accuracy of `87.2%` on the training set.
- The classification report showed precision, recall, and F1-score values for both classes (approved/declined).
  
## License

This project is licensed under the MIT License.

