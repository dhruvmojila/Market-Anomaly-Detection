# Market Anomaly Detection

Welcome to the **Market Anomaly Detection** project! This innovative tool leverages financial market data to predict market crashes and generate personalized investment strategies using cutting-edge machine learning models and advanced Large Language Models (LLMs). It offers a seamless, interactive experience for users to analyze the market and make informed investment decisions.

---

## 🚀 Live Demo & Resources

- **Project Live Demo:** [Explore the Tool](https://dhruv-mojila-market-anomaly-detection.streamlit.app/)
- **Project GitHub Repository:** [View Code on GitHub](https://github.com/dhruvmojila/Market-Anomaly-Detection)
- **Demo Video:** [Watch Project Overview](https://youtu.be/UVBFzi9LaUw)

---

## 📊 Project Overview

This project focuses on **financial market anomaly analysis** using historical data (2000-2021) and a wide array of market indicators, such as the Volatility Index (VIX), interest rates, equity indices, and more. It employs robust machine learning models to predict market anomalies and integrates an LLM-powered chatbot for personalized investment strategy recommendations.

### Key Features:
- **Predict Market Crashes:** Analyze market indicators and predict potential market crashes.
- **Generate Investment Strategies:** Use an LLM to provide customized investment advice based on user inputs and prediction results.
- **Interactive Chatbot:** Ask financial questions and get tailored responses powered by Retrieval-Augmented Generation (RAG).
- **Real-Time Insights:** Leverage a Pinecone vector database for fast and relevant data retrieval.

---

### Outline:
![flow](https://github.com/user-attachments/assets/f5cd8811-d7bb-415e-b155-f33962e7f81d)

---

## 🔍 Market Indicators & Metrics

The project evaluates five critical market metrics:

### 1. **Volatility Indicators**
- **Key Indicators:** VIX (Volatility Index), BDIY (Baltic Dry Index)
- **Relevance:** Rising volatility often signals uncertainty or fear in the market.

### 2. **Economic Sentiment and Rates**
- **Key Indicators:** USGG30YR, USGG10YR, USGG3M, EONIA, Credit Spreads
- **Relevance:** Sudden shifts in interest rates and credit spreads can indicate liquidity problems or financial stress.

### 3. **Equity Market Indicators**
- **Key Indicators:** MXUS, MXEU, MXJP, Sector-Specific Indices (e.g., CRY)
- **Relevance:** Price movements in indices can signal regional or global economic risks.

### 4. **Currencies and Commodities**
- **Key Indicators:** XAU BGNL (Gold), CRY, DXY, JPY, GBP
- **Relevance:** Gold and currency fluctuations often reflect macroeconomic shifts or geopolitical tensions.

### 5. **Liquidity and Money Market Indicators**
- **Key Indicators:** US0001M (1-Month USD LIBOR), USGG2YR, Credit Spreads
- **Relevance:** Tightening liquidity and yield curve changes can predict economic downturns.

---

## 🛠️ Models & Performance

Three machine learning models were implemented for each metric to achieve robust predictions:

### 1. **Isolation Forest**
- Designed to identify anomalies using unsupervised learning.
- **Performance:**
  - Accuracy: ~75%
  - Challenges: Moderate precision and recall for "Crash" predictions due to data imbalance.

### 2. **Logistic Regression**
- A simple yet effective supervised learning model.
- **Performance:**
  - High precision for "Normal" predictions but struggles with minority class ("Crash").

### 3. **Neural Network**
- Leverages deep learning for more complex pattern recognition.
- **Performance:**
  - Best overall accuracy (~85%) with improved balance across metrics.

---

## 🤖 LLM Integration

To complement the predictive models, an **LLM-powered chatbot** is integrated to:
- Generate investment strategies tailored to user inputs and market predictions.
- Provide real-time, context-aware answers using Retrieval-Augmented Generation (RAG).
- Retrieve relevant information from a vector database (Pinecone).

---

## 🌟 Key Challenges

1. **Domain Knowledge:** Bridging the gap in understanding financial market intricacies.
2. **Data Imbalance:** Handling minority class (market crashes) with effective techniques.
3. **Real-Time Data Availability:** Overcoming the lack of live stock market data.
4. **Performance Optimization:** Balancing precision and recall across models.

---

## 🏗️ Architecture

### Workflow:
1. **Data Preprocessing:** Clean and normalize market data.
2. **Model Training:** Train three models for each metric and combine predictions using a voting mechanism.
3. **Prediction Interface:** Allow users to input current market values and predict crash likelihood.
4. **Investment Strategy Generation:** Use the LLM to suggest strategies based on predictions and stock data.
5. **Interactive Chat:** Enable user queries and provide relevant, data-backed responses.

---

## 📚 How to Run Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/dhruvmojila/Market-Anomaly-Detection.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Market-Anomaly-Detection
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Create a `.env` file in the root directory and add the following keys:
   ```env
   GROQ_API_KEY=your_groq_api_key
   PINECONE_API_KEY=your_pinecone_api_key
   ```
5. Run the application:
   ```bash
   streamlit run app.py
   ```

---

## 🤝 Contributing
I welcome contributions!

---

## 📧 Contact
For inquiries or feedback, reach out to:
- **Author:** Dhruv Mojila
- **Email:** dhruvmojila098@gmail.com
- **LinkedIn:** [@dhruvmojila](https://www.linkedin.com/in/dhruv-mojila)

---

Unlock the future of financial market analysis with **Market Anomaly Detection**!
