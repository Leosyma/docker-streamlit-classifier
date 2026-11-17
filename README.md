# Containerized Streamlit classifier

During the Docker build, the training script generates labeled data, fits a random forest and saves it. Streamlit loads the model and predicts from values supplied by the user.

## Run locally

```sh
docker build -t streamlit-classifier .
docker run --rm -p 8501:8501 streamlit-classifier
```
