# Cryptocurrency Price Prediction and Analysis

## Project Description
The Cryptocurrency Price Prediction and Analysis project aim to utilize machine learning models to predict future price fluctuations of Bitcoin, with a focus on providing valuable insights for new and inexperienced investors. In the wake of the 2022 cryptocurrency crash, the project seeks to address the volatility and risks associated with cryptocurrency investments. The analysis involves the extraction and processing of data from various cryptocurrency markets, creating visualizations for market insights, and implementing a Random Forest Classifier for price predictions.


## Table of Contents
- [How to Install and Run the Project](#how-to-install-and-run-the-project)
- [How to Use the Project](#how-to-use-the-project)
- [Credits](#credits)

## How to Install and Run the Project
To run the project locally, follow these steps:

1. Clone the repository:
   - `git clone https://github.com/your-username/cryptocurrency-prediction.git`
   - `cd cryptocurrency-prediction`

2. Install dependencies:
   - `pip install -r requirements.txt`

3. Obtain the Coinalyze API key:
   - Visit [Coinalyze API](https://coinalyze.net/) Documentation
   - Create an account and obtain your API key

4. Add your Coinalyze API key:
   - [Notebook 1 - Data Processing](./PART%201%20-%20data%20processing%20final.ipynb)
   - Replace 'your_api_key' with your Coinalyze API key in the code

5. Run the Jupyter notebooks:
   - Execute the cells in Notebook 1, Notebook 2 and Notebook 3 to process and analyze the data

## How to Use the Project
The project provides visualizations and insights into the cryptocurrency market, specifically Bitcoin. Users can refer to the generated visualizations in the notebooks for market trends, sentiment analysis, and potential buying/selling indicators. The Random Forest Classifier model predicts price fluctuations, and users can explore the findings to make informed decisions.

## Credits
Project Contributors:

- Nicolas Pinto Galvis
- Sebastian Villada Rivera
- Henry Miranda Bastidas
## References:

- [Governors State University (Graduate Capstone Thesis)](https://opus.govst.edu/theses/132/)
- [Blekinge Institute of Technology (Bachelors Paper)](https://www.researchgate.net/publication/224098514_Learning_Machine_Learning_A_Case_Study)
- [GeeksforGeeks (Bitcoin Price Prediction using Machine Learning in Python)](https://www.geeksforgeeks.org/bitcoin-price-prediction-using-machine-learning-in-python/)
## Moving Forward
Allow users to input risk factors for a more tailored experience.
Incorporate additional model outputs (e.g., strong buy, buy at discretion) to provide more nuanced advice.
Implement risk management strategies for crypto trading.
For more insights into cryptocurrency trading, refer to this guide.

## Limitations/Problems Encountered
Comprehensive data limitations due to Coinalyze data restrictions, issues extracting from Kraken, and Binance restrictions in Canada.
Model performance might not be highly accurate, and improvements are ongoing.
Feel free to explore, contribute, and enhance the project!
