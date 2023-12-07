# Cryptocurrency Price Prediction and Analysis

## Project Description
The Cryptocurrency Price Prediction and Analysis project aim to utilize machine learning models to predict future price fluctuations of Bitcoin, with a focus on providing valuable insights for new and inexperienced investors. In the wake of the 2022 cryptocurrency crash, the project seeks to address the volatility and risks associated with cryptocurrency investments. The analysis involves the extraction and processing of data from various cryptocurrency markets, creating visualizations for market insights, and implementing a Random Forest Classifier for price predictions. To read more about our thought process for this project, visit our [Medium article](https://medium.com/@sebastian.villada_97143/is-machine-learning-the-key-to-cracking-the-crypto-conundrum-4ca767ed1aea).


## Table of Contents
- [How to Install and Run the Project](#how-to-install-and-run-the-project)
- [How to Use the Project](#how-to-use-the-project)
- [Credits](#credits)
- [References](#references)
- [Problems Encountered](#problems-encountered)

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
   - Open [Notebook 1 - Data Processing]()
   - Replace 'your_api_key' with your Coinalyze API key in the code

5. Run the Jupyter notebook 1:
   - Execute the cells in [Notebook 1 - Data Processing](Notebooks/Notebook%201%20-%20Data%20Processing.ipynb), it will return 6 CSV files (Close Volume, Funding, Liquidations, Long Short, Older BTC Closes, Open Interest)
     
6. Run the Jupyter notebook 2:
   - With the CSV files obtained from Notebook 1, execute the cells in [Notebook 2 - Data Wrangling & Visualizations](Notebooks/Notebook%202%20-%20Data%20Wrangling%20%26%20Visualizations.ipynb). Or you can use Notebook 2 directly with the provided [CSVs files](Data%20Files/CSVs%20for%20Notebook%202) (data updated on: Dec 5th, 2023)
   - This Notebook will return 1 CSV file, wrangled
  
7. Run the Jupyter notebook 3:
   - With the previous CSV file, execute all the cells on [Notebook 3 - Feature Eng. and Model Training](Notebooks/Notebook%203%20-%20Feature%20Eng.%20and%20Model%20Training.ipynb). Or like before, you can use the provided [CSV](Data%20Files/CSVs%20for%20Notebook%203) (data updated on: Dec 5th, 2023)
  

## How to Use the Project
The project provides visualizations and insights into the cryptocurrency market, specifically Bitcoin. Users can refer to the generated visualizations in the notebooks for market trends, sentiment analysis, and potential buying/selling indicators. The Random Forest Classifier model predicts price fluctuations, and users can explore the findings to make informed decisions.

## Credits
Project Contributors:

- Nicolas Pinto Galvis
- Sebastian Villada Rivera
- Henry Miranda Bastidas
## References:

- [A cryptocurrency timeline: From eCash to Ethereum](https://www.forbes.com/uk/advisor/investing/cryptocurrency/cryptocurrency-statistics/)
- [Cryptocurrency statistics 2023 - Forbes](https://www.forbes.com/uk/advisor/investing/cryptocurrency/cryptocurrency-statistics/)
- [Investopedia](https://www.investopedia.com)
- [NASDAQ](https://www.nasdaq.com)
- [Predicting the price of cryptocurrency using machine learning algorithm](https://opus.govst.edu/cgi/viewcontent.cgi?article=1131&context=theses)
- [Predicting cryptocurrency prices with machine learning algorithms: A comparative analysis](https://www.diva-portal.org/smash/get/diva2:1778251/FULLTEXT03)




## Problems Encountered
Comprehensive data limitations due to Coinalyze data restrictions, issues extracting from Kraken, and Binance restrictions in Canada.
Model performance might not be highly accurate, and improvements are ongoing.
Feel free to explore, contribute, and enhance the project!
