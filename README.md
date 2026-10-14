# Book Genre Classification

Classify a book into one of six genres from its plot summary using TF-IDF features and a trained sklearn model. A Flask app takes a summary and returns the predicted genre.

## Skills

- NLP preprocessing (cleaning, stopword removal, lemmatization, stemming)
- TF-IDF vectorization
- Multi-class text classification
- Model + vectorizer serialization
- Flask inference API/UI

## Genres

Fantasy, Science Fiction, Crime Fiction, Historical novel, Horror, Thriller.

## Dataset

`notebooks/BooksDataSet.csv` — book summaries labeled by genre.

## Run the notebook

```bash
pip install -r requirements.txt
jupyter notebook notebooks/Book_Genre_Prediction.ipynb
```

## Run the app

```bash
cd app
pip install -r ../requirements.txt
python app.py
```

Open `http://127.0.0.1:8080`, paste a plot summary, and submit.

First run downloads NLTK `stopwords` and `wordnet`.

## Structure

```
book-genre-classification/
├── notebooks/
│   ├── Book_Genre_Prediction.ipynb
│   └── BooksDataSet.csv
├── app/
│   ├── app.py
│   ├── bookgenremodel.pkl
│   ├── tfdifvector.pkl
│   └── templates/
├── requirements.txt
└── README.md
```
