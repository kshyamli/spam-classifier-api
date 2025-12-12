# spam-classifier-api

# 📱 SMS Spam Classifier: API Architecture Demo

## Overview
This project demonstrates a standard two-tier application architecture where a Machine Learning (ML) model is exposed via an interactive web interface. The solution classifies incoming SMS messages as either **SPAM** or **NOT-SPAM (HAM)** using a Multinomial Naive Bayes model.

The interface is built using **Gradio** to ensure seamless deployment and guaranteed interactivity within notebook environments like Colab, resolving cross-origin security issues common in web development.

## 🛠️ Technology Stack

* **Model:** Multinomial Naive Bayes (MNB)
* **Feature Engineering:** TF-IDF Vectorization with N-Grams
* **Data:** UCI SMS Spam Collection Dataset
* **Frontend (UI):** Gradio (used for guaranteed interactive demonstration)
* **Backend (Core Logic):** Pure Python (scikit-learn, pandas)

## 🏗️ Architecture

The system operates on the principle of separating the core logic from the user interface:

1.  **Core Logic:** The Python script handles data loading, model training, and the `predict(text)` function.
2.  **Interactive Frontend:** The Gradio interface takes user input and passes it directly to the core Python function, displaying the results instantly.

## 🚀 How to Run the Demo

### Method 1: Interactive Colab Notebook (Recommended)

The easiest way to view the working demo is to run the provided Colab notebook, which sets up the environment, trains the model, and launches the interactive UI in one cell.

1.  **Open the Notebook:** Click the link below.
    [Link to your uploaded Colab Notebook (e.g., interactive_demo_colab.ipynb)]
2.  **Run All Cells:** Go to **Runtime -> Run all**.
3.  **Use the Interface:** The working interactive UI will appear at the bottom of the output.

### Method 2: Local Python Execution (Advanced)

*(Instructions for a user who wants to install and run the Python environment locally, similar to our earlier troubleshooting.)*

1.  Clone this repository.
2.  Install dependencies: `pip install -r requirements.txt`
3.  Run the core logic: `python core_logic.py`

## 📊 Sample Output

<img width="1674" height="626" alt="Screenshot 2025-12-12 164202" src="https://github.com/user-attachments/assets/5a4f6ab6-bfb8-4a12-9480-572457c9686c" />
