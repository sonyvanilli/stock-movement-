
# Stock Movement Analysis

This project uses Python to scrape stock-related data from Telegram, preprocesses the data, and trains a machine learning model to predict stock movements. The notebook demonstrates scraping, preprocessing, training, and evaluation.

## Prerequisites

- Python 3.8 or higher
- Jupyter Notebook or Google Colab
- Libraries: `telethon`, `nest_asyncio`, `pandas`, `numpy`, `scikit-learn`

## Setup Instructions

1. Clone or download this repository.
2. Install required Python libraries using:
   ```bash
   pip install telethon nest_asyncio pandas numpy scikit-learn
   ```
3. Obtain Telegram API credentials (`api_id` and `api_hash`) from [Telegram](https://my.telegram.org/).

## Running the Notebook

1. Open the `StockMovementAnalysis.ipynb` file in Jupyter Notebook or Google Colab.
2. Follow the cells step by step:
   - **Library Installation**: Install dependencies.
   - **Telegram Scraping**: Input your `api_id` and `api_hash` to connect to Telegram.
   - **Data Preprocessing**: Prepare the data for model training.
   - **Model Training**: Train the `RandomForestClassifier` on processed data.
   - **Evaluation**: Evaluate the model's performance with accuracy metrics.

## Project Workflow

1. **Data Scraping**:
   - Connects to a Telegram channel to fetch stock-related messages.
   - Extracts relevant data (e.g., stock prices).

2. **Data Preprocessing**:
   - Cleans and formats the scraped data.
   - Extracts numerical values and removes outliers/missing values.

3. **Model Training**:
   - Splits data into training and testing sets.
   - Trains a `RandomForestClassifier` to predict stock movement.

4. **Evaluation**:
   - Computes accuracy and generates classification reports.

5. **Results Export**:
   - Saves processed data and predictions for further analysis.

## Notes

- Ensure the Telegram group/channel is accessible.
- Use the notebook's visualization for better insights into data and model performance.

## Future Improvements

- Add additional models for comparison.
- Enhance data scraping with other data sources.
- Optimize preprocessing and feature engineering.

## License

This project is licensed under the MIT License.
