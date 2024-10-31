# Spam Detection System - README

## Project Overview
This project demonstrates a **Spam Detection System** using **Logistic Regression**. The objective is to classify email messages as either spam or not spam (ham) based on their content. The system uses **Natural Language Processing (NLP)** techniques to convert textual data into numerical vectors for model training and evaluation.

## Project Workflow
1. **Data Collection and Preprocessing**  
   - Load the dataset (`mail_data.csv`).
   - Replace missing values with an empty string.
   - Encode labels:  
     - **Spam** → 0  
     - **Ham (not spam)** → 1  
2. **Data Splitting**  
   - Split the dataset into training and testing sets.
3. **Feature Extraction**  
   - Use **TF-IDF Vectorization** to convert email text into numerical vectors.
4. **Model Training**  
   - Train a **Logistic Regression** model on the training data.
5. **Model Evaluation**  
   - Evaluate the model on both training and test datasets to check the accuracy.
6. **Prediction System**  
   - Build a prediction system to classify new emails as **Spam** or **Not Spam**.

## Dependencies
- `pandas` - For data manipulation and analysis.
- `numpy` - For numerical operations.
- `scikit-learn` - For machine learning tools and evaluation metrics.

## Files in the Project
- **`mail_data.csv`**: The dataset used for training and testing the model.
- **`code.ipynb`**: The Jupyter notebook containing the complete code for the project.

## Instructions to Run the Project
1. **Clone the repository**:
   ```bash
   git clone <repository_link>
   cd <repository_folder>
   ```
2. **Install dependencies**:
   ```bash
   pip install pandas numpy scikit-learn
   ```
3. **Run the Jupyter notebook**:
   ```bash
   jupyter notebook code.ipynb
   ```
4. **Use the prediction system**:
   - Modify the `input_mail` variable to test with new messages.
   - Run the prediction cell to classify the message as **Spam** or **Not Spam**.

## Example Output
```
Input: "You got free tickets to the beach. Check the family WhatsApp!"
Output: Spam
```

## Model Performance
- **Accuracy on Training Data**: 96.70%
- **Accuracy on Test Data**: 96.59%

## Future Improvements
- Implement **Multinomial Naive Bayes** for comparison.
- Add **more datasets** to improve the model's performance.
- Deploy the model as a **web service** for real-time spam detection.

## License
This project is licensed under the MIT License.
