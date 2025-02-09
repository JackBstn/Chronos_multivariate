# Chronos for Multivariate Time Series Forecasting of Financial Data

This project aims to apply Chronos, a time series forecasting library, to multivariate distributions.
Chronos is a powerful tool for time series analysis and forecasting.
However, it is designed for univariate time series data, and it is not straightforward to apply it to multivariate time series data.
See the [Chronos GitHub repository](https://github.com/amazon-science/chronos-forecasting) for more information.

In this project, we explore various methods to pre-process, post-process, and fine-tune Chronos
for multivariate financial time series data, and ultimately apply it to a simple trading bot.

### Project Structure

The project is organized into the following subfolders:

- `models`: Contains all the machine learning and neural network models used in the project.
- `plots`: Contains all the plots and visualizations generated during the analysis.

#### Notebooks

The project includes four main Jupyter notebooks, each focusing on a different extension of the project.
We recommend to run the notebooks on Google Colab, for easier access to GPU support, better performance and compatible file-system management.

1. **chronos_multivariate_preprocessing.ipynb**:
   Apply statistical and simple machine learning methods on multivariate time series data to transform them into a univariate time series.

2. **chronos_multivariate_neural_network.ipynb**:
   Apply Chronos to all time series of the multivariate data and we combine the predictions using a simple neural network.

3. **chronos_fine_tuning.ipynb**:
   Fine-tune Chronos on a financial time series dataset to evaluate if it improves the model's performance.

4. **chronos_trading.ipynb**:
   Apply Chronos and its enhancements from the other experiments to a simple greedy trading bot.
   The bot starts with an initial budget and performs actions (HOLD, BUY, SELL) based on the prediction of the next day's market movement.

#### How to Execute the Notebooks

To execute the notebooks, you can use Google Colab, which provides a free cloud-based environment with GPU support. Follow these steps:

1. Upload the notebook to your Google Drive.
2. Open the notebook with Google Colab.
3. Ensure you have the necessary dependencies installed. You can install them using pip commands within the notebook.
4. Run the cells sequentially to execute the code.

All required dependencies are automatically installed in the first cells of each notebook.
