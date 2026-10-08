# Spam Mail Prediction

A machine learning project that classifies email and SMS messages as **spam** or **ham** (not spam). It uses **TF-IDF** text features and a **Logistic Regression** model.

## Dataset

`mail_data.csv`: about 5,570 labeled messages with two columns.

| Column | Description |
|--------|-------------|
| Category | `spam` or `ham` |
| Message | The message text |

## Workflow

1. Load the data and replace missing values with empty strings
2. Encode labels: spam = 0, ham = 1
3. Train/test split (80/20)
4. Turn text into numbers with `TfidfVectorizer` (English stop words removed, lowercase)
5. Train a Logistic Regression model
6. Measure accuracy
7. Build a predictive system: type any message and get Spam or Ham

## Results

| Data | Accuracy |
|------|----------|
| Training | ~96.7% |
| Testing | ~96.6% |

## Tech Stack

- Python
- NumPy, Pandas
- scikit-learn (`TfidfVectorizer`, `LogisticRegression`)
- Jupyter Notebook

## How to Run

```bash
git clone https://github.com/PRiNCeKUsHW/Spam-mail-prediction.git
cd Spam-mail-prediction
pip install numpy pandas scikit-learn jupyter
jupyter notebook "spam mail prediction .ipynb"
```

To test your own message, edit the `input_mail` list in the last cell and run it.

## Project Structure

```
Spam-mail-prediction/
├── mail_data.csv                  # Dataset
└── spam mail prediction .ipynb    # Preprocessing, training and prediction
```
