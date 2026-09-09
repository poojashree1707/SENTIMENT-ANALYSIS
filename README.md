# Sentiment Analysis using Hugging Face and Streamlit

## Project Overview

This project is a simple Sentiment Analysis web application built using Python, Streamlit, and Hugging Face Transformers.

The application analyzes a sentence entered by the user and identifies whether the sentiment is Positive or Negative. It also displays the confidence score of the prediction.

## Project Objective

The main objective of this project is to build an AI-powered application that can:

* Accept text from the user
* Analyze the sentiment using a pre-trained Hugging Face model
* Identify Positive sentiment
* Identify Negative sentiment
* Display the confidence score
* Provide a simple and interactive web interface

## Technologies Used

| Technology                | Purpose                     |
| ------------------------- | --------------------------- |
| Python                    | Programming language        |
| Streamlit                 | Web application framework   |
| Hugging Face Transformers | Natural Language Processing |
| PyTorch                   | Deep learning framework     |
| DistilBERT                | Pre-trained NLP model       |

## Model Used

This project uses the following pre-trained model:

`distilbert-base-uncased-finetuned-sst-2-english`

The model is based on DistilBERT and is fine-tuned for sentiment classification using the SST-2 dataset.

The model predicts two classes:

* POSITIVE
* NEGATIVE

## Project Workflow

```text
        +---------------------+
        |   User enters text  |
        +----------+----------+
                   |
                   v
        +---------------------+
        |    Streamlit UI     |
        +----------+----------+
                   |
                   v
        +---------------------+
        | Hugging Face Model  |
        |     DistilBERT      |
        +----------+----------+
                   |
                   v
        +---------------------+
        | Sentiment Prediction|
        +----------+----------+
                   |
                   v
        +---------------------+
        | Positive / Negative |
        | + Confidence Score  |
        +---------------------+
```

## Project Structure

```text
Sentiment-Analysis/
│
├── app.py
├── README.md
└── requirements.txt
```

## Application Output

<img width="1061" height="753" alt="Screenshot 2026-09-09 202925" src="https://github.com/user-attachments/assets/f5c426ce-f5ef-48bc-9de7-bb5bf61a860f" />


The screenshot shows the Sentiment Analysis application successfully identifying a positive sentence.

The user enters the sentence "The product is amazing." in the text box.
The user clicks the Analyze Sentiment button.
The Hugging Face DistilBERT model analyzes the given sentence.
The application predicts the sentiment as Positive.
The result is displayed in a green notification box.
The output shows:
Sentiment: POSITIVE
Confidence: 99.99%
The high confidence score indicates that the model is highly confident in its positive sentiment prediction.

<img width="1020" height="736" alt="Screenshot 2026-09-09 201711" src="https://github.com/user-attachments/assets/a37c5206-4304-4339-9ca9-f58bcefe5c97" />

The screenshot shows the working Sentiment Analysis web application built using Streamlit and Hugging Face.

The application provides a text box where the user can enter a sentence.
In the example, the input is "I hated this movie."
After clicking the Analyze Sentiment button, the Hugging Face model analyzes the sentence.
The application predicts the sentiment as Negative.
The result displays:
Sentiment: NEGATIVE
Confidence: 99.97%
The result is highlighted in a red notification box to clearly indicate the negative sentiment.

## Conclusion

This project demonstrates how Natural Language Processing and pre-trained Hugging Face models can be integrated with Streamlit to create a simple and interactive AI application.

It provides a beginner-friendly introduction to sentiment analysis, Transformers, and AI-powered web applications.
