# Sentiment Analysis of Movie Reviews Using LSTM

Binary sentiment classification (Positive / Negative) of IMDB movie reviews with an LSTM network
(Python, TensorFlow/Keras, NumPy, Pandas, Matplotlib, Seaborn, Scikit-learn).

Everything is in one notebook: `lstm_sentiment_analysis.ipynb` (15 steps: introduction, setup, data,
preprocessing, model, training, evaluation, prediction, error analysis, saving, conclusion, GitHub).

## Run on Windows 11 (VS Code)
```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt
code .
```
Open the notebook, select the `.venv` kernel, and choose **Run All**.

## Run on Google Colab
Upload the notebook (File > Upload notebook) and run the cells. Optional: Runtime > Change runtime type > GPU.

## Model
Embedding(10000, 64) -> LSTM(64) -> Dropout(0.3) -> Dense(32, ReLU) -> Dense(1, sigmoid).
Reviews are limited to a 10,000-word vocabulary and padded/truncated to 200 words.
80/20 train/validation split of the 25,000 training reviews; 25,000 reviews are kept for testing.

## Results
Not included on purpose. Run the notebook and record your own numbers
(accuracy, precision, recall, F1, confusion matrix) in Step 14 and here:

| Metric | My result |
|---|---|
| Accuracy | |
| Precision | |
| Recall | |
| F1-score | |
